# myvuetest

> A Vue.js project

## Build Setup

```bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# 安装 element ui

npm i element-ui -S

# 在 main.js 中添加 element ui
import ElementUI from 'element-ui'
import 'element-ui/lib/theme-chalk/index.css'

# 安装 jQuery
npm install jquery --save-dev

#在webpack.base.conf.js中配置jQuery
#第一步引用webpack
const webpack = require("webpack")

#第二步在module.exports尾部添加
  plugins: [
    new webpack.ProvidePlugin({
      jQuery: "jquery",
      $: "jquery"
    })
  ]
#第三步在main.js中引入jQuery
import $ from 'jquery'

#配置favicon图标
#第一步在index.html中添加
<link rel="shortcut icon" href="static/favicon.ico">
#第二步在webpack.dev.conf.js中下面代码段替换为
    new HtmlWebpackPlugin({
      filename: "index.html",
      template: "index.html",
      favicon: "static/favicon.ico",
      inject: true
    }),
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
