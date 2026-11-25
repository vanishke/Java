# 第十一章 GUI(图形界面编程)

> 由 `day25/第十一章_GUI(图形界面编程).ppt` 转换。

## 第 1 页　API-GUI

本页主要是图片或图形，没有可提取的文字。


## 第 2 页　本章内容

- GUI概述
- awt和swing包概述
- GUI继承体系图
- GUI案例
- 布局管理器
- 事件监听机制和适配器模式
- 常见的组件事件
- NetBeans工具介绍
- NetBeans工具使用


## 第 3 页　GUI(图形用户界面)

- GUI
  - Graphical User Interface(图形用户接口)。
  - 用图形的方式，来显示计算机操作的界面，这样更方便更直观。
- CLI
  - Command line User Interface (命令行用户接口）
  - 就是常见的Dos命令行操作。
  - 需要记忆一些常用的命令，操作不直观。
- 举例：
  - 比如：创建文件夹，或者删除文件夹等

备注：

> Java为GUI提供的对象都存在java.Awt和javax.Swing两个包中。


## 第 4 页　awt和swing包的概述

- java.awt：Abstract Window ToolKit (抽象窗口工具包)，需要调用本地系统方法实现功能。属重量级控件。
- javax.swing：在AWT的基础上，建立的一套图形界面系统，其中提供了更多的组件，而且完全由Java实现。增强了移植性，属轻量级控件。


## 第 5 页　GUI继承体系图

- 体系图

Component

Button

Container

Label

Window

Panel

Checkbox

Frame

Dialog

TextComponent

FileDialog

TextArea

TextField

备注：

> Container：为容器，是一个特殊的组件，该组件中可以通过add方法添加其他组件进来。


## 第 6 页　GUI第一个案例

- Container常用子类：Window   Panel（面板，不能单独存在。）
- Window常用子类：Frame  Dialog
- 简单的窗体创建过程：

```java
Frame  f = new Frame(“my window”);
f.setLayout(new FlowLayout());
```

  - f.setSize(300,400);//设置窗体大小
  - f.setLocation(300,200);//设置窗体出现在屏幕的位置
  - `f.setVisible(true);`


## 第 7 页　事件监听机制

- 事件源
- 事件
- 事件处理
- 事件监听器

备注：

> 通过人受伤事件讲解。


## 第 8 页　事件监听机制流程

外部动作

2  有监听器所监听的动作作于事件源上

4 将事件对象传给事件处理方式

事件对象

3 产生事件对象

事件源(组件)

监听器

监听引发事件的动作

(事件处理方式)

1  将监听器注册到事件源

备注：

> 1:确定事件源（容器或组件）
> 2:通过事件源对象的addXXXListener()方法将侦听器注册到该事件源上。
> 3:该方法中接收XXXListener的子类对象，或者XXXListener的子类XXXAdapter的子类对象。
> 4:一般用匿名内部类来表示。
> 	在覆盖方法的时候，方法的参数一般是XXXEvent类型的变量接收。
> 5:事件触发后会把事件打包成对象传递给该变量。（其中包括事件源对象。通过getSource()或者，getComponent()获取。）


## 第 9 页　适配器设计模式

- 通过适配器设计模式改进窗口关闭案例


## 第 10 页　GUI案例

- 窗体关闭事件
- 按钮点击事件
- 把数据通过文本框转移到文本域
- 鼠标事件案例
- 键盘事件案例

备注：

> 鼠标事件：更改背景色
>
> 键盘事件：录入QQ号码，如果不是数字就不让录入
> 查看API,键盘所有键都有对应的值
> char getKeyChar() 返回与此事件中的键关联的字符。
>  int getKeyCode()
> 返回与此事件中的键关联的整数 keyCode。
> static String getKeyText(int keyCode)
> 返回描述 keyCode 的 String，如 "HOME"、"F1" 或 "A"。
> static String getKeyModifiersText(int modifiers)
> 返回描述修改键的 String，如 "Shift" 或 "Ctrl+Shift"。


## 第 11 页　菜单组件

- 菜单

MenuComponent

MenuBar

MenuItem

Menu


## 第 12 页　菜单组件概述

- MenuBar,Menu,MenuItem
- 先创建菜单条，再创建菜单，每一个菜单中建立菜单项。
- 也可以菜单添加到菜单中，作为子菜单。
- 通过setMenuBar()方法，将菜单添加到Frame中。


## 第 13 页　Netbeans工具的概述和基本使用

- Netbeans工具的概述
- Netbeans工具要完成的案例
  - 模拟四则运算
  - 登录注册
