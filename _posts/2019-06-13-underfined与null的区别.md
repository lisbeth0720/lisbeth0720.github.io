---
layout:     post
title:     underfined与null的区别
subtitle:    "underfined与null的区别"
date:       2019-06-13
author:     lisbeth
header-img: img/post_02.jpg
catalog: true
tags:
    - 学习
---

之前虽然也知道这两个之间的区别，但是让我描述的话，感觉上还是说的不是很清楚。今天也详细看了一次这个知识点，现在来说说这两者间的区别。

 

null： Null类型，代表“空值”，代表一个空对象指针，使用typeof运算得到 “object”，所以你可以认为它是一个特殊的对象值。

undefined： Undefined类型，当一个声明了一个变量未初始化时，得到的就是undefined。

null是javascript的关键字，可以认为是对象类型，它是一个空对象指针，和其它语言一样都是代表“空值”，不过 undefined 却是javascript才有的。
undefined是在ECMAScript第三版引入的，为了区分空指针对象和未初始化的变量，它是一个预定义的全局变量。没有返回值的函数返回为undefined，
没有实参的形参也是undefined。

 

javaScript权威指南： null 和 undefined 都表示“值的空缺”，你可以认为undefined是表示系统级的、出乎意料的或类似错误的值的空缺，而null是表示
程序级的、正常的或在意料之中的值的空缺。

哈哈哈！！是不是感觉不是在说人话。如果和我一样不是很能听懂，请看下面。

 

javaScript高级程序设计： 在使用var声明变量但未对其加以初始化时，这个变量的值就是undefined。   null值则是表示空对象指针。

 

最后，我的理解就是： undefined是访问一个未初始化的变量时返回的值，而null是访问一个尚未存在的对象时所返回的值。因此，可以把undefined看作是空
的变量，而null看作是空的对象。

在定义一个想保存对象的变量时，就可以让该变量先保存null值，这样既能体现null是一个空指针对象，也能更好的区分null和undefined。
