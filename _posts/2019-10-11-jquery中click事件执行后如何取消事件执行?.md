---
layout:     post
title:      jquery中click事件执行后如何取消事件执行?
subtitle:    "jQuery"
date:       2019-10-11
author:     沐雪
header-img: img/wxq_01.jpg
catalog: true
tags:
    - JS
---

> 长知识篇-！

用jQuery的方式

jQuery专门为此功能提供了一个函数one。这样写就能让click这个事件只执行一次。

$("#btn3").one('click',function(){

alert('jQuey的one函数，第1次点击');

});

