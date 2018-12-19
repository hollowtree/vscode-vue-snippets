# Vue 2 Snippets for Visual Studio Code

This extension adds Vue 2 Code Snippets into Visual Studio Code.

这个插件基于最新的 Vue 2 的 API 添加了Code Snippets。

[![](https://vsmarketplacebadge.apphb.com/version/hollowtree.vue-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=hollowtree.vue-snippets)
[![](https://vsmarketplacebadge.apphb.com/installs/hollowtree.vue-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=hollowtree.vue-snippets)


### It looks like:
![](https://raw.githubusercontent.com/hollowtree/vscode-vue-snippets/master/img/show1.png)

![](https://raw.githubusercontent.com/hollowtree/vscode-vue-snippets/master/img/show2.png)


### Snippets
Including most of the API of Vue.js 2. You can type `vcom`, choose `VueConfigOptionMergeStrategies`, and press ENTER, then `Vue.config.optionMergeStrategies` appear on the screen.

插件的 Snippets 如下表格所示，比如你可以键入 `vcom` 然后按上下键选中 `VueConfigOptionMergeStrategies` 再按Enter键，就输入了`Vue.config.optionMergeStrategies`了。

As shown in the table below, snippet `vmData` has body like `${this, vm}.$data` will provides choice `this.$data` and `vm.$data` to you.

如下表所示，`vmData` 的内容是 `${this, vm}.$data`，这表明这个 snippet 会提供 `this.$data` and `vm.$data` 两种选项供你选择。

| Prefix | JavaScript Snippet Content |
| ------ | ------------ |
| `import` | `import ... from ...` |
| `newVue` | `new Vue({...})` |
| `VueConfigSilent` | `Vue.config.silent = true` |
| `VueConfigOptionMergeStrategies` | `Vue.config.optionMergeStrategies` |
| `VueConfigDevtools` | `Vue.config.devtools = true` |
| `VueConfigErrorHandler` | `Vue.config.errorHandler = function (err, vm, info) {...}` |
| `VueConfigWarnHandler` | `Vue.config.warnHandler = function (msg, vm, trace) {...}` |
| `VueConfigIgnoredElements` | `Vue.config.ignoredElements = ['']` \
| `VueConfigKeyCodes` | `Vue.config.keyCodes` |
| `VueConfigPerformance` | `Vue.config.performance = true` |
| `VueConfigProductionTip` | `Vue.config.productionTip = false` |
| `vueExtend` | `Vue.extend( options )` |
| `VueNextTick` | `Vue.nextTick( callback, [context] )` |
| `VueNextTickThen` | `Vue.nextTick( callback, [context] ).then(function(){ })` |
| `VueSet` | `Vue.set( target, key, value )` |
| `VueDelete` | `Vue.delete( target, key )` |
| `VueDirective` | `Vue.directive( id, [definition] )` |
| `VueFilter` | `Vue.filter( id, [definition] )` |
| `VueComponent` | `Vue.component( id, [definition] )` |
| `VueUse` | `Vue.use( plugin )` |
| `VueMixin` | `Vue.mixin({ mixin })` |
| `VueCompile` | `Vue.compile( template )` |
| `VueVersion` | `Vue.version` |
| `data` | `data() { return {} }` |
| `watchWithOptions` | `key: { deep: true, immediate: true, handler: function () { } }` |
| `vmData` | `${this, vm}.$data` |
| `vmProps` | `${this, vm}.$props` |
| `vmEl` | `${this, vm}.$el` |
| `vmOptions` | `${this, vm}.$options` |
| `vmParent` | `${this, vm}.$parent` |
| `vmRoot` | `${this, vm}.$root` |
| `vmChildren` | `${this, vm}.$children` |
| `vmSlots` | `${this, vm}.$slots` |
| `vmScopedSlots` | `${this, vm}.$scopedSlots.default({})` |
| `vmRefs` | `${this, vm}.$refs` |
| `vmIsServer` | `${this, vm}.$isServer` |
| `vmAttrs` | `${this, vm}.$attrs`|
| `vmListeners` | `${this, vm}.listeners`|
| `vmWatch` | `${this, vm}.$watch( expOrFn, callback, [options] )` |
| `vmSet` | `${this, vm}.$set( object, key, value )` |
| `vmDelete` | `${this, vm}.$delete( object, key )` |
| `vmOn` | `${this, vm}.$on( event, callback )` |
| `vmOnce` | `${this, vm}.$once( event, callback )` |
| `vmOff` | `${this, vm}.$off( [event, callback] )` |
| `vmEmit` | `${this, vm}.$emit( event, […args] )` |
| `vmMount` | `${this, vm}.$mount( [elementOrSelector] )` |
| `vmForceUpdate` | `${this, vm}.$forceUpdate()` |
| `vmNextTick` | `${this, vm}.$nextTick( callback )` |
| `vmDestroy` | `${this, vm}.$destroy()` |
| `renderer` | `const renderer = require('vue-server-renderer').createRenderer()` |
| `createRenderer` | `createRenderer({ })` |
| `preventDefault` | `preventDefault();` |
| `stopPropagation` | `stopPropagation();` |

<br />

| Prefix | HTML Snippet Content |
| ------ | ------------ |
| `template` | `<template></template>` |
| `script` | `<script></script>` |
| `style` | `<style></style>` |
| `vText` | `v-text=msg` |
| `vHtml` | `v-html=html` |
| `vShow` | `v-show` |
| `vIf` | `v-if` |
| `vElse` | `v-else` |
| `vElseIf` | `v-else-if` |
| `vForWithoutKey` | `v-for` |
| `vFor` | `v-for="" :key=""` |
| `vOn` | `v-on` |
| `vBind` | `v-bind` |
| `vModel` | `v-model` |
| `vPre` | `v-pre` |
| `vCloak` | `v-cloak` |
| `vOnce` | `v-once` |
| `key` | `:key` |
| `ref` | `ref`|
| `slotA` | `slot=""`|
| `slotE` | `<slot></slot>`|
| `slotScope` | `slot-scope=""`|
| `component` | `<component :is=''></component>`|
| `keepAlive` | `<keep-alive></keep-alive>` |
| `transition` | `<transition></transition>` |
| `transitionGroup` | `<transition-group></transition-group>` |
| `enterClass` | `enter-class=''`|
| `leaveClass` | `leave-class=''`|
| `appearClass` | `appear-class=''`|
| `enterToClass` | `enter-to-class=''`|
| `leaveToClass` | `leave-to-class=''`|
| `appearToClass` | `appear-to-class=''`|
| `enterActiveClass` | `enter-active-class=''`|
| `leaveActiveClass` | `leave-active-class=''`|
| `appearActiveClass` | `appear-active-class=''`|
| `beforeEnterEvent` | `@before-enter=''`|
| `beforeLeaveEvent` | `@before-leave=''`|
| `beforeAppearEvent` | `@before-appear=''`|
| `enterEvent` | `@enter=''`|
| `leaveEvent` | `@leave=''`|
| `appearEvent` | `@appear=''`|
| `afterEnterEvent` | `@after-enter=''`|
| `afterLeaveEvent` | `@after-leave=''`|
| `afterAppearEvent` | `@after-appear=''`|
| `enterCancelledEvent` | `@enter-cancelled=''`|
| `leaveCancelledEvent` | `@leave-cancelled=''`|
| `appearCancelledEvent` | `@appear-cancelled=''`|

<br />

| Prefix | Vue Router Snippet Content |
| ------ | ------------ |
| `routerLink` | `<router-link></router-link>` |
| `routerView` | `<router-view></router-view>` |
| `to` | `to=""` |
| `tag` | `tag=""` |
| `newVueRouter` | `const router = newVueRouter({ })` |
| `routerBeforeEach` | `router.beforeEach((to, from, next) => { }` |
| `routerBeforeResolve` | `router.beforeResolve((to, from, next) => { }` |
| `routerAfterEach` | `router.afterEach((to, from) => { }` |
| `routerPush` | `router.push()` |
| `routerReplace` | `router.replace()` |
| `routerGo` | `router.back()` |
| `routerBack` | `router.push()` |
| `routerForward` | `router.forward()` |
| `routerGetMatchedComponents` | `router.getMatchedComponents()` |
| `routerResolve` | `router.resolve()` |
| `routerAddRoutes` | `router.addRoutes()` |
| `routerOnReady` | `router.onReady()` |
| `routerOnError` | `router.onError()` |
| `routes` | `routes: []` |
| `beforeEnter` | `beforeEnter: (to, from, next) => { }` |
| `beforeRouteEnter` | `beforeRouteEnter (to, from, next) { }` |
| `beforeRouteLeave` | `beforeRouteLeave (to, from, next) { }` |
| `scrollBehavior` | `scrollBehavior (to, from, savedPosition) { }` |

<br />

| Prefix | Vuex Snippet Content |
| ------ | ------------ |
| `newVuexStore` | `const store = new Vuex.Store({ })` |

| Prefix | Nuxt.js Snippet Content |
| ------ | ------------ |
| `nuxt` | `<nuxt/>` |
| `nuxtChild` | `<nuxt-child/>` |
| `nuxtLink` | `<nuxt-link to=""/>` |
| `asyncData` | `asyncData() {}` |

### Supported languages
* vue(.vue)
* HTML(.html)
* javascript(.js)
* typescript(.ts)
* pug(.pug)

### Base on
[vue-syntax-highlight (vue.tmLanguage)](https://github.com/vuejs/vue-syntax-highlight/blob/master/vue.tmLanguage)

--------------------------------------
##### 2018/12/19 (0.1.10)
* Update sinppets (like `watchWithOptions` / `asyncData` / `nuxt` / `nuxtChild` / `nuxtLink` and so on)

##### 2018/09/04 (0.1.9)
* Update sinppets

##### 2018/06/24 (0.1.8)
* Update sinppets

##### 2018/06/05 (0.1.7)
* Update sinppets, add choices(`this` and `vm`) to snippets that begin with `vm`.

##### 2018/05/22 (0.1.6)
* Update sinppets

##### 2017/09/17 (0.1.5)
* Fix and update sinppets

##### 2017/03/12 (0.1.1)
* Add support .pug files (thanks to [Gregory Bass](https://github.com/GriNAME))

##### 2017/01/01 (0.1.0)
* Update some sinppets

##### 2016/12/31 (0.0.10)
* Update newest api sinppets (like `v-else-if` / `Vue.config.ignoredElements` and so on)
* Fix a bug (before: `vm.off`,after:`vm.$off`)

##### 2016/12/15 (0.0.9)
* Update newest syntax highlight file

##### 2016/11/13 (0.0.8)
* Add some snippets
* Change this extension's logo to vue's logo
* Update readme

##### 2016/10/18 (0.0.7)
* Fix `v-for` snippet (thanks to [Daniel D](https://github.com/djx339))

##### 2016/10/18 (0.0.6)
* Publish failed

##### 2016/10/16 (0.0.5)
* Fix this extension can not be downloaded with the latest version(1.6.1) of VS code

##### 2016/10/15 (0.0.4)
* Update readme

##### 2016/09/30 (0.0.1)
* Add code snippets
* Add syntax highlight
