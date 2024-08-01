>当我们构建越来越大型的应用时，需要处理的Javascript代码量也呈指数级增长。
我们开始遇到性能瓶颈--使用Javascript开发的工具通常需要很长时间才能启动开发服务器（启动项目）。即使是用HMR（热更新），文件修改后的效果也需要几秒才能在浏览器反应（热更新迟缓）。影响开发效率。

```
yarn start

yarn dev

npm run dev 

npm run start

```

webpack支持多种模块化，AST抽象语法分析的工具，分析出你写的js文件有哪些导入和导出操作构建工具是运行在服务端的。

```javascript

//这一段代码最终会到浏览器里去运行
const lodash =require("lodash");//commonjs规范
import Vue from "vue";//es6 module

//webpack是允许我们这么写的
//webpack转换的结果：
const lodash=webpack_require("lodash);
const Vue = webpack_require("vue);

```

