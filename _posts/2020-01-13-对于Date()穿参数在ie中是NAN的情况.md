---
layout:     post
title:      对于Date()穿参数在ie中是NAN的情况
subtitle:    "浏览器兼容性问题"
date:       2020-01-13
author:     lisbeth
header-img: img/2019-12-19-backhround.jpg
catalog: true
tags:
    - 对于Date()穿参数在ie中是NAN的情况
---

>大多数人想要改造这个世界，但却罕有人想改造自己。

一开始我写的时间格式是"2020,1,3"  即var timeNum = getBeforeDate('2020，1，3')
这个时间在谷歌、火狐里均是正常的，但是在测试的时候发现在IE中报错是NAN
之后经过一番探索发现是IE中对于Date的时间格式过于严格，必须是“-”相连，并且月份日份为单数的时候必须添加0；
即
var timeNum = getBeforeDate('2020-01-03');
日常挖坑-跳坑-
但是收获颇多。
