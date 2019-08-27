#  Scorpio  
预览  https://tls1234.github.io/Scorpio/dist/index#/index
## 技术栈
> [vue](https://cn.vuejs.org/v2/guide/)、[vue-router](https://router.vuejs.org/zh-cn/essentials/getting-started.html)、[vuex](https://vuex.vuejs.org/zh-cn/getting-started.html)、[axios（请求库）](https://github.com/axios/axios)、[muse-ui（移动端UI库）](http://www.muse-ui.org/#/install)

> [vue-awesome-swiper（轮播图）](https://github.com/surmon-china/vue-awesome-swiper)、[vue-progressbar（加载进度条）](https://github.com/hilongjw/vue-progressbar)、[lib-flexible（淘宝适配库）](https://github.com/amfe/lib-flexible)、[mockjs（数据模拟）](http://mockjs.com/)、[Material Icons（google图标）](http://google.github.io/material-design-icons/)

> [ES6/7（JS语法）](https://github.com/lukehoban/es6features)、[Stylus（css预处理器）](https://github.com/stylus/stylus)、[ESlint（JS风格规范）](https://github.com/standard/standard/blob/master/docs/RULES-zhcn.md)、[webpack3（资源处理）](https://github.com/webpack/webpack)


## 功能

- [x] 全站内播放（单页面优点）
- [x] 播放 & 暂停 & 下一首
- [x] 播放模式： 默认、随机播放、单曲循环、列表循环
- [x] 播放进度条 & 可调节播放进度
- [x] 播放列表 & 可删除播放列表 & 可点击切换音乐
- [x] 一键播放
- [ ] 弹幕 （太耗移动web性能和个人时间，暂不实现啦）
- [ ] 手机铃声（好像只有app获取用户手机权限才能实现，web暂不可能实现，如果可以实现请告知我）

## 目录结构

``` bash
├── build                        // 构建相关  
├── config                       // 配置相关
├── src                          // 源代码
│   ├── assets                   // 样式、图标等静态资源
│   ├── components               // 全局公用组件
│   |   ├── banner.vue           // banner组件
│   |   ├── error.vue            // 错误组件
│   |   ├── list.vue             // 列表组件
│   |   ├── loading.vue          // 加载组件
│   |   ├── musicBar.vue         // 音乐条组件
│   |   ├── sheet.vue            // 模态框组件
│   ├── config                   // 全局公用方法
│   |   ├── cache.js             // 缓存方法
│   |   ├── fetch.js             // 请求方法
│   |   ├── util.js              //  工具方法
│   ├── mock                     // mock数据
│   ├── page                   
│   |   ├── detail               //  详情页
│   |   ├── index                //  首页
│   ├── router                   // 路由
│   ├── store                    // 状态管理
│   ├── App.vue                  // 入口页面
│   └── main.js                  // 入口 加载组件 初始化等
├── static                       // 空文件夹，只作为github保留
├── .babelrc                     // babel-loader 配置
├── eslintrc.js                  // eslint 配置项
├── .gitignore                   // git 忽略项
├── index.html                   // html模板
└── package.json                 // package.json
```

## 安装运行

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8088
npm run dev

# build for production with minification
npm run build
