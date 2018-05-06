---
layout:post
title:Github page jekyll搭建个人博客遇到的问题
description:jekyll serve启动失败的一种情况
tag: blog
---

当本地执行jekyll serve是，提示报错：

![img](file:///C:\Users\ChangHe\AppData\Local\Temp\ksohtml\wps308D.tmp.jpg)

这是提示本地端口4000被占用。

我们需要找到占用该端口的线程，关掉就好了



 

在本地命令行cmd下按照如下操作执行



![img](file:///C:\Users\ChangHe\AppData\Local\Temp\ksohtml\wps308E.tmp.jpg)

该指令让我们得到现有的线程占用端口的情况。

查找到被占用的端口



![img](file:///C:\Users\ChangHe\AppData\Local\Temp\ksohtml\wps308F.tmp.jpg)

该指令得到占用该端口的是那个线程

找到线程的名称。



![img](file:///C:\Users\ChangHe\AppData\Local\Temp\ksohtml\wps3090.tmp.jpg)

在任务管理器的服务栏，找到该线程，禁止掉就好了
