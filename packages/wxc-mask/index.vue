<!--
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->
<!-- Created by Tw93 on 16/10/25. -->
<!-- Updated by Tw93 on 17/01/06. -->
<!--A Mask.-->

<template>
  <div class="container">
    <wxc-overlay :show="show && hasOverlay"
                 v-if="show"
                 v-bind="mergeOverlayCfg"
                 :can-auto-close="overlayCanClose"
                 :opacity='opacity'
                 @wxcOverlayBodyClicking="wxcOverlayBodyClicking"
                 @wxcOverlayBodyClicked="wxcOverlayBodyClicked"></wxc-overlay>
    <div ref="wxc-mask"
         class="wxc-mask"
         v-if="show"
         :hack="shouldShow"
         :style="maskStyle">
      <div :style="contentStyle">
        <slot></slot>
      </div>
      <div class="mask-bottom"
           :style="{ width: width + 'px' }"
           @click="closeIconClicked"
           v-if="showClose">
        <image :src="closeIcon"
               aria-label="关闭"
               class="mask-close-icon"></image>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .container {
    position: fixed;
    width: 750px;
    /*兼容H5异常*/
    z-index: 99999;
  }

  .wxc-mask {
    position: fixed;
  }

  .mask-bottom {
    width: 100px;
    height: 100px;
    background-color: transparent;
    justify-content: center;
    align-items: center;
  }

  .mask-close-icon {
    width: 64px;
    height: 64px;
  }
</style>

<script>
  const animation = weex.requireModule('animation');
  import WxcOverlay from '../wxc-overlay';

  export default {
    components: { WxcOverlay },
    props: {
      height: {
        type: [String, Number],
        default: 800
      },
      width: {
        type: [String, Number],
        default: 702
      },
      top: {
        type: Number,
        default: 0
      },
      show: {
        type: Boolean,
        default: false
      },
      showClose: {
        type: Boolean,
        default: false
      },
      duration: {
        type: [String, Number],
        default: 300
      },
      hasOverlay: {
        type: Boolean,
        default: true
      },
      hasAnimation: {
        type: Boolean,
        default: true
      },
      timingFunction: {
        type: Array,
        default: () => (['ease-in', 'ease-out'])
      },
      overlayCfg: {
        type: Object,
        default: () => ({
          hasAnimation: true,
          timingFunction: ['ease-in', 'ease-out'],
          canAutoClose: true,
          duration: 300,
          opacity: 0.6
        })
      },
      borderRadius: {
        type: [String, Number],
        default: 0
      },
      overlayCanClose: {
        type: Boolean,
        default: true
      },
      maskBgColor: {
        type: String,
        default: '#ffffff'
      },
      opacity: {
        type: [Number, String],
        default: 0.6
      },
    },
    data: () => ({
      closeIcon: 'https://gw.alicdn.com/tfs/TB1qDJUpwMPMeJjy1XdXXasrXXa-64-64.png',
      maskTop: 264,
      opened: false
    }),
    computed: {
      mergeOverlayCfg () {
        return {
          ...this.overlayCfg,
          hasAnimation: this.hasAnimation
        }
      },
      maskStyle () {
        const { width, height, showClose, hasAnimation, opened, top } = this;
        const newHeight = showClose ? height - 0 + 100 : height;
        const { deviceHeight, deviceWidth, platform } = weex.config.env;
        const _deviceHeight = deviceHeight || 1334;
        const isWeb = typeof (window) === 'object' && platform.toLowerCase() === 'web';
        const navHeight = isWeb ? 0 : 130;
        const pageHeight = _deviceHeight / deviceWidth * 750 - navHeight;
        return {
          width: width + 'px',
          height: newHeight + 'px',
          left: (750 - width) / 2 + 'px',
          top: (top || (pageHeight - height) / 2) + 'px',
          opacity: hasAnimation && !opened ? 0 : 1
        }
      },
      contentStyle () {
        return {
          width: this.width + 'px',
          backgroundColor: this.maskBgColor,
          height: this.height + 'px',
          borderRadius: this.borderRadius + 'px'
        }
      },
      shouldShow () {
        const { show, hasAnimation } = this;
        hasAnimation && setTimeout(() => {
          this.appearMask(show);
        }, 50);
        return show;
      }
    },
    methods: {
      closeIconClicked () {
        this.appearMask(false);
      },
      wxcOverlayBodyClicking () {
        if (this.hasAnimation) {
          this.appearMask(false);
          this.$emit('wxcOverlayBodyClicking', {});
        }
      },
      wxcOverlayBodyClicked () {
        if (!this.hasAnimation) {
          this.appearMask(false);
          this.$emit('wxcOverlayBodyClicked', {});
        }
      },
      needEmit (bool = false) {
        this.opened = bool;
        !bool && this.$emit('wxcMaskSetHidden', {});
      },
      appearMask (bool, duration = this.duration) {
        const { hasAnimation, timingFunction } = this;
        const maskEl = this.$refs['wxc-mask'];
        if (hasAnimation && maskEl) {
          animation.transition(maskEl, {
            styles: {
              opacity: bool ? 1 : 0
            },
            duration,
            timingFunction: timingFunction[bool ? 0 : 1],
            delay: 0
          }, () => {
            this.needEmit(bool);
          });
        } else {
          this.needEmit(bool);
        }
      }
    }
  };
</script>
