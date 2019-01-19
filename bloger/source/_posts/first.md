---
title: vue-cli生成vue项目
date: 2019-01-17 15:54:13
tags:
---

![avatar](https://raw.githubusercontent.com/langhuonan/wechat/master/mdimg/day1/1.jpg)


### 全局安装 vue-cli
1.$ cnpm install --global vue-cli 

如果已经安装过了就不用安装了，这里我前面的项目已经安装过了，所以直接从第二步开始
<!-- more -->
### my-project为自定义项目名
2.$ vue init webpack my-project

需要注意的是项目的名称不能大写，不然会报错
![avatar](https://raw.githubusercontent.com/langhuonan/wechat/master/mdimg/day1/2.png)


### 项目初始化时会询问一些安装项，可以根据自己的需求选择
![avatar](https://raw.githubusercontent.com/langhuonan/wechat/master/mdimg/day1/1.png)

Project name (my-project) ==>项目名称（我的项目）



Project description (A Vue.js project) ==>项目描述一个Vue.js 项目



 Author 作者（你的名字）



nstall vue-router? (Y/n) ==>是否安装Vue路由，也就是以后是spa（但页面应用需要的模块）yes

Use ESLint to lint your code? (Y/n) ==>使用 ESLint 到你的代码？ （Y [ yes ] / N [ no ]）此处建议选no，如果不是按照ESLint风格，编译时就会报错（就是这里坑了我，找半天没发现逻辑问题）



Pick an ESLint preset (Use arrow keys) ==>选择一个预置ESLint（使用箭头键） 



Setup unit tests with Karma + Mocha? (Y/n) ==>设置单元测Karma + Mocha？ （Y/ N）



Setup e2e tests with Nightwatch? (Y/n) ==>设置端到端测试，Nightwatch？这里需要选yes，否则会报websocket的错误 （Y/ N）Y

3.最后一步就是安心等待啦
![avatar](https://raw.githubusercontent.com/langhuonan/wechat/master/mdimg/day1/0.png)

完成后运行npm run Dev项目就运行起来啦

![avatar](https://raw.githubusercontent.com/langhuonan/wechat/master/mdimg/day1/0.jpg)

**注：**

Vue取消eslint语法限制

在build/webpack.base.conf.js文件中，注释或者删除掉：module->rules中有关eslint的规则

![avatar](https://raw.githubusercontent.com/langhuonan/wechat/master/mdimg/day1/4.png)
