---
layout:     post
title:      了解onFocus="this.blur()"
subtitle:    "onFocus="this.blur()""
date:       2019-09-27
author:     沐雪
header-img: img/post-bg-six.jpg
catalog: true
tags:
    - js
---

> 未来可期！

onFocus="this.blur()"

onFocus即获取焦点的意思，而blur却是失去焦点的意思，因此onFocus="this.blur()"的通俗理解就是：当获取焦点时立即失去焦点，听起来的确有点绕，那么这种方法到底有何使用价值呢？

1、当你在使用一个文本框时，且在某种情况下有想让文本框不能操作（无法输入文本），这时可以使用onFocus="this.blur()"，即你不能把光标放在这个文本框上——不能输入任何文本的文本框。

2、可以通过onFocus="this.blur()"来消除链接后的焦点虚线框，不过似乎还存在着浏览器兼容问题。

一个小小的知识点！
