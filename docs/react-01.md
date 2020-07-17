# React 入门
## 目标及路径
### 目标
主要目标是通过对 `React.js` 基础原理及开发方式的学习，掌握 React 的基本开发方法，能够开发简单的 React 应用。并且对前端工具链的结构、功能、配置、基础原理有相应了解。
### 学习路径
- 学习 React 基础原理，跟随 [React.js 小书](http://huziketang.mangojuice.top/books/react/) 走一遍原理，并且能够使用原生 `JavaScript` 实现一遍 React 核心轮子；
- 搭建一个 `React Demo` 项目，可以使用命令行工具搭建，搭建过程中手动添加相应前端工具链，了解工具链组合，并且认知各个工具的基础能力；
- 开发基础的组件，通过造一些小轮子熟悉 React 的开发方法，并且通过这样的过程熟悉相应的语法，能够看懂 React App 应用；
- 开发一个简单的管理页面，熟悉使用 React.js 开发一个项目的基本流程，同时学习 `React 工具栈`，了解工具栈中各个工具都解决了什么问题，以及相应的用途。
## 项目搭建
### 项目生成
使用官方推荐的 `create-react-app` 来生成项目即可，可以参考 [相关链接](https://create-react-app.dev/docs/getting-started) 进行项目骨架生成；
### 目录结构
生成的默认项目骨架如下所示，其中，`src` 目录为源代码目录，后续配置 `webpack` 打包，其默认的源码路径就是 `src`，且入口文件为 `index.js`。
```
└── react-learning
    ├── README.md
    ├── docs
    │   └── react-01.md
    ├── package-lock.json
    ├── package.json
    ├── public
    │   ├── favicon.ico
    │   ├── index.html
    │   ├── logo192.png
    │   ├── logo512.png
    │   ├── manifest.json
    │   └── robots.txt
    └── src
        ├── App.css
        ├── App.js
        ├── App.test.js
        ├── index.css
        ├── index.js
        ├── logo.svg
        ├── serviceWorker.js
```
## 工具链
前端工具链众多，目前待了解和学习的工具链有如下一些：
1. 包管理工具：`npm` 是较为流行的包管理工具，主要需要熟悉 npm 的基本用法及原理；
2. 打包工具：`webpack` 是较为流行的前端打包工具，主要需要熟悉 webpack 的基本用法及基本原理。使用 `create-react-app` 创建的 React 应用没有直接暴露出 webpack 的配置文件，`package.json` 中也没有显式依赖 webpack，是因为 webpack 已经被包装到 `react scripts` 中，故需要同时了解该工具的用法及原理；
3. 编译工具：`Babel` 是较为流行的编译工具，主要是把旧版浏览器不支持的新 `JavaScript` 语法编译为旧版浏览器支持的语法，私以为，这从另外一个方面也体现出了 JS 最初设计的不合理，以及前端开发面对多浏览器的痛苦之处。