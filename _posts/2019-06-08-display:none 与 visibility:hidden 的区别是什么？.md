---
layout:     post
title:    display:none 与 visibility:hidden 的区别是什么？
subtitle:    "display:none 与 visibility:hidden 的区别是什么？"
date:       2019-06-08
author:     lisbeth
header-img: img/post_01.jpg
catalog: true
tags:
    - 学习
---
> 永远不要停止对知识的探索！

display : 隐藏对应的元素但不挤占该元素原来的空间。
visibility: 隐藏对应的元素并且挤占该元素原来的空间。
即是，使用 CSS display:none 属性后，HTML 元素（对象）的宽度、高度等各种属性值都将
“丢失”;而使用 visibility:hidden 属性后，HTML 元素（对象）仅仅是在视觉上看不见（完
全透明），而它所占据的空间位置仍然存在
