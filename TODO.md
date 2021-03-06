## 剩余工作

### 开发工作

 - 自动打包插件 ★★★★★

    > 收集页面的JS与CSS引用或require依赖进行打包。优先使用pack设置进行打包处理，将其余零散的资源文件以及依赖打成一个包。

 - 前端模块化  ★★★★☆
 
    > 主要是改进[fis-postpackager-modjs](https://github.com/fouber/fis-postpackager-modjs)，使其收集所有同步异步依赖，将样式文件依赖直接全部注入头部，将同步脚本资源注入底部，同时调整[modjs-todo-demo](https://github.com/fouber/modjs-todo-demo/)，加入样式表的引用。

 - Angularjs方案 ★★★☆☆
 
    > 使用modjs+fis-postpackager-modjs+angularjs管理angularjs项目的静态资源依赖和加载

 - FIS增加插件依赖自动安装功能  ★★☆☆☆
 
    > 需要考虑到插件版本问题，修改目前找不到插件的提示，给出安装指引

### 文档调整

 - 完整版快速上手 ★★★★★
 
    > 完整版快速上手用于展示fis release的关键参数和能力以及fis server的本地调试能力

 - 目录定制快速上手 ★★★★★
 
    > 与目前的roadmap.path文档不同，以实际项目和需求为例，给出目录定制说明

 - 插件安装快速上手  ★★★★★
 
 - 自动打包快速上手 ★★★★★
 
    > 使用自动打包插件和快速上手DEMO

 - 进阶知识内容与结构调整  ★★★★☆
 
    将目前的语言能力、运行原理、静态资源管理等内容重新整理放在此处

 - FAQ补全 ★★★★☆

 - 插件定制指南 ★★★★☆
 
    > 原理性文章继续引用原有内容，但是需要添加每个扩展点的参数以及具体含义和用法DEMO。此外由于不是所有用户都愿意发布插件，还需要对插件能力进行降级，给出直接在fis-conf.js中扩展的办法。

 - 官方插件文档补全 ★★★☆☆
    
    > 补全插件的配置说明

 - 插件准入标准制订 ★★★☆☆
    
    > 建立插件准入的文档、功能标准，用于接入社区插件

 - 静态资源管理实现指南 ★★☆☆☆
 
    > 进阶知识，指导静态资源管理的实现

 - 前后端结合实现指南 ★★☆☆☆

    > 进阶知识，指导后端渲染模板以及后端模块化与后端的结合方法

### DEMO需求

 - 前端模块化DEMO  ★★★★☆

    > 可以在已有的TODO-DEMO上修改，但是需要添加样式文件依赖，DEMO中应该将自动打包功能也整合进去

 - 快速上手DEMO调整 ★★★★★
 
    > 目前已经完成了简版的快速上手，但是DEMO需要调整为一个更加传统的前端项目，而不是目前用于展示语言能力DEMO，需要有一定的资源量用于后面的打包等功能的演示。

 - Angularjs方案DEMO ★★★☆☆
 
