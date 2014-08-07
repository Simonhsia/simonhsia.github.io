---
layout: post
title: "制作 OSX 安装 U 盘"
author: simon
excerpt: "OSX 安装 U 盘制作记要"
tags: [OSX]
---

### 准备U盘

1. 用「磁盘工具」分区 U 盘，

2. 格式为「Mac OS 扩展」、方案选项为「GUID 分区表」

3. 制作

### 源文件

1. 在安装 App 右键「显示包内容」

2. 装载 `Contents/SharedSupport/InstallESD.dmg`

### 制作U盘

1. 在「磁盘工具」选择 U 盘 > 恢复

2. 在「源磁盘」输入 `/Volumes/OS X Install ESD/BaseSystem.dmg`

「# BaseSystem.dmg 是隐藏文件，也可以在终端用 `open` 装载 dmg」

3. 拖拽 U 盘至「目的磁盘」

4. 恢复

5. 恢复完成后，进入U盘目录 `/Volumes/OS X Base System/System/Installation` 删除 `Package` 替身身文件

6. 拷贝  `/Volumes/OS X Install ESD/Packages`  文件夹至 U 盘 `/Volumes/OS X Base System/System/Installation` 目录下

### 完成 
