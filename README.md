# NodeJS_Projects

表示安装成功
npm -v 

npm 升级
npm install npm -g

使用npm命令安装模块
$ npm install <Module Name>
以下实例，我们使用 npm 命令安装常用的 Node.js web框架模块 express:

$ npm install express
安装好之后，express 包就放在了工程目录下的 node_modules 目录中，因此在代码中只需要通过 require('express') 的方式就好，无需指定第三方包路径。

var express = require('express');


全局安装与本地安装
npm 的包安装分为本地安装（local）、全局安装（global）两种，从敲的命令行来看，差别只是有没有-g而已，比如
npm install express          # 本地安装
npm install express -g   # 全局安装


产看安装信息
npm list -g

产看某个模块的版本号
$ npm list grunt


使用 package.json
package.json 位于模块的目录下，用于定义包的属性。node_modules/express/package.json

卸载模块
$ npm uninstall express
$ npm ls 查看是否已经卸载

更新模块
我们可以使用以下命令更新模块：
$ npm update express

搜索模块
使用以下来搜索模块：
$ npm search express

创建模块
创建模块，package.json 文件是必不可少的。我们可以使用 NPM 生成 package.json 文件，生成的文件包含了基本的结果。
$ npm init

接下来我们就用以下命令来发布模块：
$ npm publish


查看其它命令的使用方法
npm help install。