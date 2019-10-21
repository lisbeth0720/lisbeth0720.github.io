---
layout:     post
title:      input中name与id的区别
subtitle:    "移动端布局"
date:       2019-10-21
author:     沐雪
header-img: img/wxq_03.jpg
catalog: true
tags:
    - CSS
---

> 探索知识的道路注定是漫长的！

一直很困惑，表单里面input标签有id和name,它们之间到底有什么区别自己很少去想，只知道一般的场景该怎么使用，今天就在网上搜索了一下，自己也总结一下。为什么有了ID还要有Name呢?其实ID就像是一个人的身份证号码，而Name就像是他的名字，ID显然是唯一的，而Name是可以重复的。

　　**name与id的还有区别是：**
  
id要符合标识的要求,比如大小写敏感,最好不要包含下划线(因为不兼容CSS)。而name基本上没有什么要求,甚至可以用数字。
补充：name主要是表单元素里才有的属性。通过js的document.表单名称.文本框.value来获取文本框的值，其中的表单名称和文本框名称指的是name,而非表单元素例如div，span等是没有name属性的，而id属性是任何一个HTML元素都会有的。当你需要用js获取非表单元素对象是就得用document.getElementByIdx("id")

　　**name在以下用途是不能替代的：**
   
1. 表单(form)的控件名，提交的数据都用控件的name而不是id来控制。因为有许多name会同时对应多个控件,比如checkbox和radio, 而id必须是全文档中唯一的。此外浏览器会根据name来设定发送到服务器的request。因此如果用id，服务器是无法得到数据的。
2. frame和window的名字,用于在其他frame或window指定target。

　　*以下两者可以通用，但是强烈建议用id不要用name：*
  
1. 锚点，通常以前写作<a name="myname">,现在可以用任何的元素id来指定:```<div id="myid">```。

　*以下情况只能用id：*
  
1. label与form控件的关联,

```
    <label for="MyInput">My Input</label>
     <input id="MyInput" type="text"> ```

     for属性指定与label关联的元素的id,不可用name替代。

2. CSS的元素选择机制，以#MyId的方式指定应用样式的元素,不能用name替代。
3. 脚本中获得对象:
IE支持在脚本中直接以id(而不是name)引用该id标识的对象。例如上面的input,要在脚本中获得输入的内容,可以直接以MyInput.value来获得。
如果用DOM的话,则用document.getElementById("MyInput").value,如果要用name的话,通常先得到包含控件的form,例如document.forms[0]，然后从form再引用name,注意这样得到的是经过计算后将发送给服务器的值。

