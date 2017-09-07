轻量级的的视差引擎Parallax.js
  http://modernizr.cn/ 检测浏览器支持h5情况
  https://codepen.io/  canvas插件
 -
 -sublime插件  colorHighlighter
 --------------------------------------------------------
 -html css js prettify 配置
 +--------------------------------------------------------------------
 +sublime插件  1. colorHighlighter
 +2.html css js prettify 配置
  {
    // Details: https://github.com/victorporof/Sublime-HTMLPrettify#using-your-own-jsbeautifyrc-options
    // Documentation: https://github.com/einars/js-beautify/
 @@ -63,3 +62,41 @@ html css js prettify 配置
  修改了"html"、"css"、"js"的"indent_size"，我的代码缩进为2个空格
  ---------------------------------------------------------------------------
  chrome插件 colorZilla 、 view image info
 +---------------------------------------------------------------------------
 +---基于node环境 简单安装webpack---
 +webpack：一个模块加载器、打包工具（js，css，图片）
 +
 +安装：
 +1.安装命令环境 cnpm install webpack -g
 +2.验证ok webpack --version
 +3.新建文件目录、package.json 工程文件（需要依赖的模块、库描述）  npm .init
 +4.安装本地webpack  cnpm install webpack -D / --save -dev
 +
 +
 +例子
 +index.html  页面
 +entry.js  入口文件
 +编写代码
 +命令：webpack entry.js bundle.js
 +
 +自动解决依赖：
 +	默认支持commonJs规范
 +
 +webpack 默认只支持js文件
 +
 +*需要用到加载器（loader）
 +loader类似一种转化器，他可以把一个东西转成另一个
 +
 +css文件：style-loader  css-loader
 +
 +安装cnpm install  style-loader css-loader -D
 +
 +注意：在webpack中，多个loader加载 用！连接
 +
 +配置 webpack.config.js 配置需要的出入口、loader
 +
 +webpack  开发环境下编译
 +webpack -p  开发环境压缩
 +webpack -w  监听文件改动，自动编译（速度快）
 +webpack -d  开启source maps 
 +webpack -wdp
