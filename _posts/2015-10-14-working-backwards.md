---
layout: post
title: "亚马逊的Working Backwards方法"
description: ""
category: 
tags: [Amazon]
---
{% include JB/setup %}
在亚马逊使用的细粒度服务方法中，服务不只代表软件结构，更代表组织构架。
这些服务有着很强的[代码所有权模型](https://orgpatterns.wikispaces.com/CodeOwnership)，这使得它们各自的团队规模都很小，从而各个团队更容易创新。
从某种意义上来说，这些服务更像是同一个大公司下的若干小创业公司。
不管是对外还是队内，每一个服务都把重心放在他们的客户身上。
为了保证一个服务能满足客户的需求，我们遵循一种叫**Working Backwards**的方法。
这种方法从最终客户出发，以与传统开发顺序相反的方向推导出具体需求，直到获得一些列能满足目标的最小技术需求。
我们的目标就是通过持续明确的关注客户，使得整个事情变得简单。

产品定义过程用这样的方式反着进行：
首先，我们写下发布新产品所需的文档（新闻稿和FAQ）；然后一步一步向最终的实现推进。

**Working Backwards**产品定义过程就是充实概念、清晰地阐述我们最终的将要运作或者构建的产品。
它通常有四个步骤：

1. **从写新闻稿开始**。新闻稿用一种简单的方式描述了产品的功能和优点。它需要非常的清晰、有重点。先写下新闻稿可以弄清楚这个世界是如何看待这个产品的——不只是我们内部如何看待它。
2. **写常见问题（FAQ）**。让我们来给新闻稿订下的骨架增添血肉。记下写新闻稿中遇到的问题；记下与其他人分享新闻稿过程中被问到的问题；回答这个产品为什么好；假设自己是使用这个产品的人，思考你会遇到的问题。
3. **定义用户体验**。精确地描述客户使用产品过程中的各种细节。对于有用户界面的产品，我们要设计客户使用的每一个界面原型。对于web service，我们写下包含想象中客户使用产品的代码片段用例。这一步的目标就讲清楚，客户如何使用本产品解决问题。
4. **写用户手册**。用户手册是客户用来查看产品说明和用法的。用户手册通常有客户使用产品需要知道的三个部分，概念、如何使用、参考。对于有多种角色的产品，我们要写若干份用户手册。

当我们把新闻稿、FAQ、原型和用户手册都设计之后，我们就能看到计划开发的产品是多么清晰。
我们有了一系列文档来向亚马逊的其他团队介绍新产品。
这时候，所有的团队就对我们将要构建的产品有了共同的预期。

翻译自 [Working Backwards](http://www.allthingsdistributed.com/2006/11/working_backwards.html)

这里有更多的资料解释**Working Backwards**：

1. [Ian McAllister的精彩quora回答](https://www.quora.com/What-is-Amazons-approach-to-product-development-and-product-management/answer/Ian-McAllister)给出了一个新闻稿大纲。
2. [Amazon Product Management, Working Backwards](http://brendansterne.com/2013/11/21/amazon-product-management-working-backwards/)比较了Working Backwards和Lean Startup的区别