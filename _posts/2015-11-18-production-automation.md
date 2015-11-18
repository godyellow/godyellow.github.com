---
layout: post
title: "生产线部署运维自动化"
description: ""
category: 
tags: [devops][nodejs]
---
{% include JB/setup %}
最近在撸后台服务，前期开发，经常要更新生产线。频繁的重新部署带来不少重复劳动，遂随手撸了个小脚本：

 1. bitbucket的master收到push后，发webhook到生产线监听服务；
 2. 监听服务把生产线停止；
 3. 更新代码库；
 4. 更新依赖、编译；
 5. 重新启动生产线。

github上竟然没有还在维护中的小工具来做这件事情。