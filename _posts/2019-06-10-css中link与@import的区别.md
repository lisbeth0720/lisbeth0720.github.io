---
layout:     post
title:     CSS 中 link 和@import 的区别是：
subtitle:    "CSS 中 link 和@import 的区别是："
date:       2019-06-10
author:     lisbeth
header-img: img/post_02.jpg
catalog: true
tags:
    - 学习
---
> 书山有路勤为径，徐海无涯苦做舟！

Link 属于 html 标签，而@import 是 CSS 中提供的在页面加载的时候，link 会同时被加载，而@import 引用的 CSS 会在页面加载完成后才会加
载引用的 CSS。

@import 只有在 ie5 以上才可以被识别，而 link 是 html 标签，不存在浏览器兼容性问题。

Link 引入样式的权重大于@import 的引用（@import 是将引用的样式导入到当前的页面中）。
