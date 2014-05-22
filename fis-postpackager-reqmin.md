fis-postpackager-reqmin
=============================

## 概述

在编译期收集页面的资源依赖，并将资源打包，将打包结果注入页面

## 功能

 - 支持[fis-postprocessor-require-async](https://github.com/xiangshouding/fis-postprocessor-require-async)，分析file.extras.async，但是所有异步样式资源均同步加载。
 - 支持人工干预打包结果，即可以预先设置pack打包指定资源，则插件只会将剩余资源打成一个包。
 - 支持对脚本和样式表声明的资源依赖进行收集和打包替换。

## 流程

 1. 分析页面脚本和样式声明，将显示资源与页面依赖合并
 1. 分析页面独立脚本，移动到页面底部
 1. 递归遍历依赖，记录命中的打包资源A
 1. 将所有没有命中打包资源的资源按照依赖顺序进行合并B
 1. 将A+B的资源注入至页面

## 额外

与[fis-postpackager-modjs](https://github.com/fouber/fis-postpackager-modjs)整合需要将**样式资源**从resourceMap中剔除