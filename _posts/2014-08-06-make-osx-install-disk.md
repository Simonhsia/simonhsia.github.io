---
layout: post
title: "制作 OSX 安装 U 盘"
author: simon
excerpt: "OSX 安装 U 盘制作记要"
tags: [OSX]
---

1. 准备U盘

 a.用「磁盘工具」分区 U 盘，

 b.格式为「Mac OS 扩展」、方案选项为「GUID 分区表」

 c.制作

2. 源文件

a.在安装 App 右键「显示包内容」

b.装载 `Contents/SharedSupport/InstallESD.dmg`

3.制作U盘

a.在「磁盘工具」选择 U 盘 > 恢复

b.在「源磁盘」输入 `/Volumes/OS X Install ESD/BaseSystem.dmg`

「# BaseSystem.dmg 是隐藏文件，也可以在终端用 `open` 装载 dmg」

c.拖拽 U 盘至「目的磁盘」

d.恢复

e.恢复完成后，进入U盘目录 `/Volumes/OS X Base System/System/Installation` 删除 `Package` 替身身文件

f.拷贝  `/Volumes/OS X Install ESD/Packages`  文件夹至 U 盘 `/Volumes/OS X Base System/System/Installation` 目录下

完成 
