# Change Log

## 0.8.0
- [!]From alibaba/weex-ui to [apcahe/incubator-weex-ui](https://github.com/apache/incubator-weex-ui) 

## 0.7.1
- [+] [wxc-slider-bar](https://apache.github.io/incubator-weex-ui/#/cn/packages/slider-bar) add `wxcSliderBarTouchEnd` event.
- [!] Fixed [wxc-mask](https://apache.github.io/incubator-weex-ui/#/cn/packages/mask) jitter bug when inputting.
- [!] Fixed the problem that the QR code does not display when debugging.

## 0.7.0
- [-] Remove alipay util,Preventing audit issues [issue/467](https://github.com/apache/incubator-weex-ui/issues/467)
- [!] [wxc-tab-bar](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-tab-bar) add `supportXBar` param.

## 0.6.16
- [+] [wxc-pan-item](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-pan-item/) add `extId` when  pan. [issue/441](https://github.com/apache/incubator-weex-ui/issues/441)

## 0.6.15
- [!] [wxc-swipe-action](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-swipe-action/)fix delete the last data item, then click on another item to report the error.
- [!] [wxc-slider-bar](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-slider-bar/) fix dynamically assign value to value, then slide back to return value
- [!] [wxc-radio](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-radio/) fix the selected item cannot be modified when modifying the list array

## 0.6.14
- [!] [wxc-swipe-action](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-swipe-action/) adds slot labels, extended style and height attributes

## 0.6.13
- [!] Fixed[wxc-overlay](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-dialog/)problem on[wxc-tab-bar](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-tab-bar/)
- [+] add a new componet named wxc-swipe-action
- [!] Fix [wxc-button](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-button/) displaying style problem, add isHighlight attribute to control whether button is highlighted or not.

## 0.6.12
- [!] Fixed set transparency issues [wxc-lightbox](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-lightbox/).
- [!] Fixed set transparency issues [wxc-mask](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-mask/).
- [!] Fixed cannot click, the component cannot modify the internal style [wxc-special-rich-text](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-rich-text/).
- [!] Fixed click no highlighting question [wxc-button](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-button/).

## 0.6.11
- [!] Fixed the shake when change disabled about [wxc-button](https://apache.github.io/incubator-weex-ui/#/packages/wxc-button/).
- [!] Fixed the line-height bug about [wxc-stepper](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-stepper/).
- [!] Fixed the loopedIndex bug about [wxc-ep-slider](https://apache.github.io/incubator-weex-ui/#/packages/wxc-ep-slider/).

## 0.6.10

- [!] Fixed the `lines` bug about [wxc-popover](https://apache.github.io/incubator-weex-ui/#/packages/wxc-popover/) when in web.  [issue/384](https://github.com/apache/incubator-weex-ui/issues/384)
- [!] Fixed the `sourceData` warning about [wxc-city](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-city/) when searching. [issue/382](https://github.com/apache/incubator-weex-ui/issues/382)
- [!] Fixed the `btnStyle` style cannot cover about [wxc-button](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-button/). [issue/390](https://github.com/apache/incubator-weex-ui/issues/390)
- [+] Add Weex and Bindingx DingTalk Group.

## 0.6.9
- [!] Fixed the bug about [wxc-loading](https://apache.github.io/incubator-weex-ui/#/packages/wxc-loading/) When `need-mask` is false.
- [-] Remove the special treatment for weex-toolkit in [with-weex-toolkit](https://apache.github.io/incubator-weex-ui/#/docs/with-weex-toolkit).

## 0.6.8
- [+] [wxc-tab-page](https://apache.github.io/incubator-weex-ui/#/packages/wxc-tab-page/) supports more settings about tab-item, More can see [here]((https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-tab-page/))
- [+] [wxc-lightbox](https://apache.github.io/incubator-weex-ui/#/packages/wxc-tab-page/) add  params about `index` and `interval`
- [!] [wxc-rich-text](https://apache.github.io/incubator-weex-ui/#/packages/wxc-rich-text/)  remove the old hack about wxc-special-rich-text

## 0.6.7
- [!] Modifying the location attribute of loading [pull/323](https://github.com/apache/incubator-weex-ui/pull/323)
- [!] English document grammar correction [pull/329](https://github.com/apache/incubator-weex-ui/pull/329)、[pull/330](https://github.com/apache/incubator-weex-ui/pull/330)
- [+] New judgement method about iPhoneXS Max/ iPhoneXR  in util [utils](https://apache.github.io/incubator-weex-ui/#/packages/utils/) [pull/337](https://github.com/apache/incubator-weex-ui/pull/337)
- [!] Update the npm version of querystringify and url-parse [pull/329](https://github.com/apache/incubator-weex-ui/pull/329)
- [+] [wxc-button](https://apache.github.io/incubator-weex-ui/#/packages/wxc-button/) add a green theme [pull/291](https://github.com/apache/incubator-weex-ui/pull/291)
- [+] [wxc-indexlist](https://apache.github.io/incubator-weex-ui/#/packages/wxc-indexlist/) add a  `need-animation` param to disable the index animation [issue/341](https://github.com/apache/incubator-weex-ui/issues/341)
- [!] Fixed the bug about [wxc-slider-bar](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-slider-bar/) When drag can still be dragged after Android dragging the slider. [issue/331](https://github.com/apache/incubator-weex-ui/issues/331)
- [+] [wxc-minibar](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-minibar/) add bar-style param to cover style  [issue/326](https://github.com/apache/incubator-weex-ui/issues/326)

## 0.6.6
- [!] Fixed the padding undefined bug for [wxc-tab-page](https://apache.github.io/incubator-weex-ui/#/packages/wxc-tab-page/)   [issue/320](https://github.com/apache/incubator-weex-ui/issues/320)
- [!] Fixed the standOut Value bug for [wxc-popup](https://apache.github.io/incubator-weex-ui/#/packages/wxc-popup/)     [issue/319](https://github.com/apache/incubator-weex-ui/issues/319)

## 0.6.5
- [+] [`wxc-button`](https://apache.github.io/incubator-weex-ui/#/packages/wxc-button/) supports to set the disabled style for replace
- [!] Fixed the link click callback for [`wxc-rich-text`](https://apache.github.io/incubator-weex-ui/#/packages/wxc-rich-text/)  [issue/298](https://github.com/apache/incubator-weex-ui/issues/298)
- [+] [wxc-city](https://apache.github.io/incubator-weex-ui/#/packages/wxc-city/) supports show or hidden nav header by `show-nav-header` param. [issue/294](https://github.com/apache/incubator-weex-ui/issues/294)
- [+] [wxc-tab-bar](https://apache.github.io/incubator-weex-ui/#/packages/wxc-tab-bar/) supports set selected when is not tabView. [issue/292](https://github.com/apache/incubator-weex-ui/issues/292)
- [+] [wxc-popover](https://apache.github.io/incubator-weex-ui/#/packages/wxc-popover/) supports to replace text style. [issue/289](https://github.com/apache/incubator-weex-ui/issues/289)

## 0.6.4
- [+] [`wxc-searchbar`](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-searchbar/) supports the type of setting the keyboard return key.  [issues/287](https://github.com/apache/incubator-weex-ui/issues/287)
- [!] Fixed the [wxc-slider-bar](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-slider-bar/) bug about position. [issues/282](https://github.com/apache/incubator-weex-ui/issues/282)
- [+] [wxc-slider-bar](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-slider-bar/) supports dynamic modification of data and style in real time display.
- [!] Fixed the bug about [wxc-button](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-button/) when set the `type`. [issues/268](https://github.com/apache/incubator-weex-ui/issues/268)
- [+] Fixed the bug about [wxc-grid-select](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-grid-select/) when using more than one.
- [!] Fixed the bug about [`wxc-ep-slider`](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-ep-slider/) when slide to last one. [issues/277](https://github.com/apache/incubator-weex-ui/issues/277)

## 0.6.3
- [!] Fixed the bug about [`wxc-minibar`](https://apache.github.io/incubator-weex-ui/#/packages/wxc-minibar/) when setting right slot.  [issue/263](https://github.com/apache/incubator-weex-ui/issues/263)
- [+] [`wxc-ep-slider`](https://apache.github.io/incubator-weex-ui/#/packages/wxc-ep-slider/) supports pull more  by setting `pull-more` slot.
- [!] Fixed the bug about [wxc-icon](https://apache.github.io/incubator-weex-ui/#/packages/wxc-icon/) when requesting font source.   [issues/253](https://github.com/apache/incubator-weex-ui/issues/253)
- [+] [wxc-popup](https://apache.github.io/incubator-weex-ui/#/packages/wxc-popup/) supports setting `stand-out`.  [issue/251](https://github.com/apache/incubator-weex-ui/issues/251)
- [+] supports to auto generate entry `index.js`. [pull/259](https://github.com/apache/incubator-weex-ui/pull/259)
- [!] Fixed the bug about [wxc-searchbar](https://apache.github.io/incubator-weex-ui/#/packages/wxc-searchbar/) barStyle return default value is `undefined`.  [pull/255](https://github.com/apache/incubator-weex-ui/pull/255)
- [+] [wxc-result](https://apache.github.io/incubator-weex-ui/#/packages/wxc-result/) supports to add customer result type.  [pull/252](https://github.com/apache/incubator-weex-ui/pull/252)

## 0.6.2
- [+] [`utils`](https://apache.github.io/incubator-weex-ui/#/packages/utils/) more powerful， add `objToParams`、`paramsToObj`、`getPageHeight`、`getScreenHeight` new functions, More you can see [utils/index.js](https://github.com/apache/incubator-weex-ui/blob/master/packages/utils/index.js).
- [!] Fixed the bug about [`wxc-ep-slider`](https://apache.github.io/incubator-weex-ui/#/packages/wxc-ep-slider/) when only two sliders  [pull/248].(https://github.com/apache/incubator-weex-ui/pull/248)
- [!] Fixed the bug about [`wxc-searchbar`](https://apache.github.io/incubator-weex-ui/#/packages/wxc-searchbar/) when setting up custom styles and background conflicts at the same time  [issues/242](https://github.com/apache/incubator-weex-ui/issues/242)/[pull/245](https://github.com/apache/incubator-weex-ui/pull/245)
- [+] [`wxc-mask`](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-mask/) Supports `top` param to control height at the top of the distance.  [issues/240](https://github.com/apache/incubator-weex-ui/issues/240)/[pull/241](https://github.com/apache/incubator-weex-ui/pull/241)
- [!] Fixed the demo bug about [`wxc-popover`](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-popover/)  [pull/236](https://github.com/apache/incubator-weex-ui/pull/236)

## 0.6.1
- [+] [`wxc-tab-page`](https://apache.github.io/incubator-weex-ui/#/packages/wxc-tab-page/) add `wxc-full-page` of immersion full screen effect, more you can see the component document.
- [+] [`wxc-tab-page`](https://apache.github.io/incubator-weex-ui/#/packages/wxc-tab-page/) add a param about `need-slider`.
- [!] Fixed the bug about `import {BindEnv} from 'weex-ui'`.
- [!] [wxc-cell](https://apache.github.io/incubator-weex-ui/#/packages/wxc-cell/)  supports setting extra content.
- [!] Fixed the show about [`wxc-slider-bar`](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-slider-bar/) in web and iOS
- [+] [`wxc-refresher`](https://apache.github.io/incubator-weex-ui/#/cn/packages/wxc-refresher/) supports refresh and pullingdown event.

## 0.6.0
- [+] [wxc-button](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-button/README.md) supports more `type` settings, remove `normal`/ `highlight`，add new `type` ahout `white` and `blue`，new button `size` settings, pay attention to the upgrade.
- [!] Solve the problem of too big packaging bundle of bindingx，`Binding related judgments` are transferred from `Utils.env` to `BindEnv`，pay attention to the upgrade. [issue 191](https://github.com/apache/incubator-weex-ui/issues/191)
- [+] New Binding component: [`wxc-refresh`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-refresh/README.md), at the present stage of beta, suggestions are welcome.
- [-] Remove the hints for `default style of the component` in weex-vue-loader high version.  [issue 198](https://github.com/apache/incubator-weex-ui/issues/189)
- [+] [wxc-popover](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-popover/README.md) support animation.  [pr 184](https://github.com/apache/incubator-weex-ui/pull/184/files)
- [+] [wxc-searchbar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-searchbar/README.md) support setting `bar-style` style to cover theme color.
- [!] [wxc-rich-text](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-rich-text/README.md) enhanced compatibility with iPad and Android.
- [+] Document update for Faq and Binding.


## 0.5.3
- [!] [wxc-city](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-city/README.md) support not to display the location, direct incoming `currentLocation` is empty.
- [+] [wxc-checkbox](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-checkbox/README.md) add `has-top-border`/`has-bottom-border` for whether show top-border or bottom-border.
- [+] [wxc-progress](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-progress/README.md) add `bar-radius` for setting border-radius.

## 0.5.2
* [!] Using `rebind()` to be compatible older version about [wxc-ep-slider](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-ep-slider/README.md).
* [+] [wxc-searchbar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-searchbar/README.md) allow translation of "cancel" button label
* [!] Fix the `overlay-can-close` bug about [`wxc-mask`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-tab-mask/README.md).

## 0.5.0
* [+] [wxc-tab-page](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-tab-page/README.md)、[wxc-ep-slider](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-ep-slider/README.md)、[wxc-slider-bar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-slider-bar/README.md) support [Bindingx](https://alibaba.github.io/bindingx/). 🎉🎉
* [-] Remove `rebind()` about [wxc-ep-slider](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-ep-slider/README.md).
* [!] Fix the `props` bug about [`wxc-city`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-city/README.md).
* [+] Compatible with android and add more demo for [wxc-popover](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-popover/README.md).

## 0.4.1
* [+] New component: [`wxc-popover`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-popover/README.md). 🎉🎉
* [+] [wxc-city](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-city/README.md)、[wxc-page-calendar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-calendar/README.md) supports for `model` animation.
* [+] [wxc-tab-page](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-tab-page/README.md)、[wxc-tab-bar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-tab-bar/README.md) support to set margin between iconFont and text.
* [+] [wxc-loading](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-city/README.md) supports to set mask for preventing incorrect clicking.
* [+] [wxc-simple-flow](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-simple-flow/README.md) supports to set multi-line title.

## 0.4.0

* [+] Stronger about [wxc-city](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-city/README.md)，it's easier to use, no need to configure a lot of parameters.
* [!] Optimization of GitHub Readme.
* [+] Add a Chinese version of [Changelog](https://github.com/apache/incubator-weex-ui/blob/master/CHANGELOG_cn.md)
* [+] Add more FQA.
* [+] Merge pull request from committer.

## 0.3.13

* [!] Fix the `slot` bug about [`wxc-tab-bar`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-tab-bar/README.md).
* [!][wxc-indexlist](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-indexlist/README.md) supports fully custom style. [issue 132](https://github.com/apache/incubator-weex-ui/issues/132)
* [+] Add a post about [`Weex + Ui - Weex Conf 2018`](https://apache.github.io/incubator-weex-ui/#/cn/weex-ui-weex-conf-2018)`, Welcome to [translate](https://github.com/apache/incubator-weex-ui/blob/master/docs/weex-ui-weex-conf-2018.md) it.

## 0.3.12

* [+] Add `happypack` to improve the speed of build.
* [+] Add a show case of [weex-ui](https://github.com/tw93/weex-ui-demo).
* [+][wxc-stepper](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-stepper/README.md) supports dynamic modification of default values [issue126](https://github.com/apache/incubator-weex-ui/issues/126).
* [!] Fix the style bug about [wxc-grid-select](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-grid-select/README.md) [issue123](https://github.com/apache/incubator-weex-ui/issues/123).

## 0.3.11

* [+][`wxc-tab-bar`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-tab-bar/README.md) supports fully customizable navigation header using slot
* [!] Fixed the dynamic update bug about [wxc-radio](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-radio/README.md).
* [!] Fixed the example code error about [wxc-result](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-result/README.md). [issue112](https://github.com/apache/incubator-weex-ui/issues/112).
* [!] Fix the bug about [wxc-mask](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-mask/README.md) that will hidden when updating. [issue111](https://github.com/apache/incubator-weex-ui/issues/111).
* [!] Fix the iconfont bug about [`wxc-tab-bar`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-tab-bar/README.md).
* [+] The official website supports user editing and directly copy example code.

## 0.3.10

* [+] New component: [`wxc-icon`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-icon/README.md). 🎉🎉
* [+] New component: [`wxc-city`](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-city/README.md).
* [-] Remove the default position relative style.
* [+] `wxc-indexlist` add a head slot. [issue105](https://github.com/apache/incubator-weex-ui/issues/105)
* [+] `wxc-tab-bar` [supports for IPhoneX](https://img.alicdn.com/tfs/TB1_qrtkf2H8KJjy0FcXXaDlFXa-768-354.png).

## 0.3.9

* [+] `wxc-minibar` supports slot.
* [+] Stronger about [wxc-rich-text](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-rich-text/README.md),do not need post the width and height for a icon.
* [+] Add a [FQA](https://apache.github.io/incubator-weex-ui/#/docs/fqa).

## 0.3.8

* [+] The [wxc-tab-bar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-page-bar/README.md) and [wxc-tab-page](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-page-bar/README.md) support for `iconFont`.
* [!] Fixed the custom configuration bug about [wxc-radio](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-radio/README.md). [issue 89](https://github.com/apache/incubator-weex-ui/issues/89).
* [!] Fixed the blank display about [wxc-button](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-button/README.md).

## 0.3.7

* [!] Fixed the height calculation error about[wxc-tab-bar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-page-bar/README.md).
* [+] Util function Enhancement.
* [!] Modify the configuration of webpack.

## 0.3.4

* [+][wxc-radio](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-radio/README.md#api)、[wxc-checkbox](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-checkbox/README.md#checkboxlist) add a `config` param for changing the style and icon.
* [!][wxc-result](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-result/README.md) using general theme instead of `fliggy theme`.
* [!][wxc-button] using `red/yellow` instead of `taobao/fliggy`.
* [+] Add a [`chat`](https://apache.github.io/incubator-weex-ui/) of the website.

## 0.3.3

* [+][wxc-tab-bar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-page-bar/README.md) supports `bedge`、`dot` setting.
* [+] Add component [demo page](https://apache.github.io/incubator-weex-ui/docc/demo.html) of the website.

## 0.3.2

* [!] Organize all component documents.
* [!] Some of the optimizations on the [website](https://apache.github.io/incubator-weex-ui/).
* [!] Fixed some component export error in some env [issue 70](https://github.com/apache/incubator-weex-ui/issues/70).

## 0.3.1

* [+] wxc-page-calendar add a showHeader params.
* [!] Correct the minibar function callback.

## 0.3.0

* [+] New component: [wxc-tab-bar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-page-bar/README.md) 🎉🎉
* [-] Remove all demo Internal characteristics of Alibaba.

## 0.2.9

* [+] Support for IPhoneX.
* [!] The code format follows ESlint.
* [+] Stronger about [wxc-page-calendar](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-page-calendar/README.md).
* [+] Document official website. 🎉🎉

## 0.2.8

* [+] Accessibility of components. 🎉🎉

## 0.2.7

* [+] Stronger about [wxc-tab-page](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-tab-page/README.md).
* [!] Updated the development packages.
* [!] Supplement the README.

## 0.2.6

* [!] Fixed the wxc-dialog bug.

## 0.2.3

* [-][#44](https://github.com/apache/incubator-weex-ui/issues/44) Remove the `overlay-can-close` prop in `wxc-mask`.
* [-][#45](https://github.com/apache/incubator-weex-ui/issues/45) Remove the useless style in `wxc-cell`.
* [!] Fixed the `npm run start` .

## 0.2.2

* [!] Fix image link problem.

## 0.2.1

* [+] Stronger about [wxc-ep-slider](https://github.com/apache/incubator-weex-ui/blob/master/packages/wxc-ep-slider/README.md).
* [!] Extraction of [common functions](https://github.com/apache/incubator-weex-ui/blob/master/packages/utils/README.md).

## 0.2.0

* [!] Update reference mode.
* [!] Normalized structure.
* [!] Fixed part of the component in some environments that cannot be used.

## 0.1.3

* [+] Fix syntax highlighting.
* [!] Fixed wxc-indexlist bug from [issues/16](https://github.com/apache/incubator-weex-ui/issues/16).
* [!] Normalize wxc-searchbar,wxc-minibar function name.

## 0.1.2

* [!] fixed the link jump bug.
* [!] Modify the usage documentation for some components.

## 0.1.1

* [!] Improve component usage documentation.

## 0.1.0

* [+] The first full version. 🎉🎉
