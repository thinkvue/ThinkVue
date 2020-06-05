<!--
 * @Author: thinkvue@thinkvue.cn
 * @URL: https://thinkvue.com
 * @Date: 2020-06-05 08:13:53
 * @LastEditors: thinkvue@thinkvue.cn
 * @LastEditTime: 2020-06-05 08:14:18
 * @FilePath: \\ThinkVue\\readme.md
 * @Description:  
--> 
ThinkVue
===============

## 项目介绍

ThinkVue是一套基于Vue全家桶（Vue2.x + Vue-router2.x + Vuex）+  Thinkphp + Uni-App的前后端分离框架，支持APP、手机端、各种小程序、快应用等一套代码全平台覆盖。

ThinkVue构建了菜单管理、权限节点、部门/岗位管理、用户组/用户管理等基础功能，并且提供了示例功能代码，可以快速上手，敏捷开发。


## 主要适用技术栈
* 后端框架：ThinkPHP 5.0.x/ThinkPHP 5.1.x
* 前端MVVM框架：Vue.JS 2.x
* 开发工作流：Webpack 1.x
* 路由：Vue-Router 2.x
* 数据交互：Axios
* 代码风格检测：Eslint
* UI框架：Element-UI 1.1.6(Vue)/ColorUI(Uni-APP)
* JS函数库：Lodash
* 图标库：[阿里iconfont](https://www.iconfont.cn/)


## 开发依赖

* vue <https://vuefe.cn/v2/guide/>
* element-ui@1.1.3  <http://element.eleme.io/1.1/#/zh-CN/component/installation>
* axios  <https://github.com/mzabriskie/axios>
* fontawesome <http://fontawesome.io/icons/>
* js-cookie  <https://github.com/js-cookie/js-cookie>
* lockr  <https://github.com/tsironis/lockr>
* lodash  <http://lodashjs.com/docs/>
* moment  <http://momentjs.cn/>
* Uni-APP <https://uniapp.dcloud.io/>
* iconfont <https://www.iconfont.cn/>



## 数据交互

数据交互通过RESTful架构实现，用户验证由放在header中AuthKey辨别，其中AuthKey是由Clint随机产生的32位随机字符串，有效时长在config/app.php中设置，默认为3600秒。Vue端通过Axios发送请求，Uni-APP通过uni.request发送请求，两者都进行了预处理，不需要手动干预会话。  

Chromium核心的相关浏览器跨域请求会预请求OPTION，确认服务器开启了跨域才会第二次数据请求，因此需要开启miss路由或者开启所有URL的Option响应，显然前者更优雅。

## 环境要求

* LAMP/LNMP/WAMP
* MySQL >= 5.6
* PHP >= 7.1
* PDO PHP Extension
* MBstring PHP Extension
* CURL PHP Extension


## 调试工具

- 封包:　Chrome + [Tabbed Postman](https://chrome.google.com/webstore/detail/tabbed-postman-rest-clien/coohjcphdfgbiolnekdpbcijmhambjff)
- Vue:　[vscode](https://code.visualstudio.com/)
- Uni-APP:　[HBuilder](https://dcloud.io/hbuilderx.html)
- 微信：　[TBS Studio](https://thinkvue.cn/2020/05/13/chrome-wechat/)
- ThinkPHP:　[vscode](https://code.visualstudio.com/)

## 使用许可

[MIT](https://opensource.org/licenses/MIT)