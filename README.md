# Java 基础班课程资料

本仓库是一套按天排列的 Java 基础课程，目标是 27 天掌握 Java 基础。每天一个目录，里面是当天笔记、课件和示例工程。课件页脚为「北京传智播客教育」。

版权归原作者所有，欢迎自由转载-非商用-非衍生-保持署名和链接。

笔记和课件都是 Markdown。

## 目录

- [文档说明](#docs)
- [每天学什么](#daily)
  - 基础语法：[day01 环境与 HelloWorld](#day01) · [day02 变量与运算符](#day02) · [day03 流程控制](#day03) · [day04 循环与方法](#day04) · [day05 数组](#day05)
  - 面向对象：[day06 类与对象](#day06) · [day07 构造方法与 static](#day07) · [day08 继承与多态](#day08) · [day09 抽象类与接口](#day09) · [day10 包与内部类](#day10)
  - 常用类：[day11 Eclipse 与 Object](#day11) · [day12 String](#day12) · [day13 StringBuffer 与包装类](#day13) · [day14 正则与日期](#day14)
  - 集合：[day15 Collection 与 List](#day15) · [day16 泛型](#day16) · [day17 Set](#day17) · [day18 Map](#day18)
  - IO：[day19 File 与异常](#day19) · [day20 IO 入门](#day20) · [day21 字符流](#day21) · [day22 其他流](#day22)
  - 多线程与界面：[day23 多线程](#day23) · [day24 单例模式](#day24) · [day25 GUI](#day25) · [day26 作业](#day26)
- [复习笔记](#review)
- [示例工程](#projects)

<a id="docs"></a>

## 文档说明

- 课堂笔记按原来的条目写成标题和列表，成段的 Java 代码放进代码块。
- PPT 按页保留标题、要点和演讲者备注。每页重复的页脚「北京传智播客教育 www.itcast.cn」没有写入正文。纯图片或图形页只留了一句说明，图片本身没有导出。
- Word 里的对照表、测试题和作业转成了标题、列表和表格。
- 程序运行时读写的数据文件仍保留，例如 `user.txt`、`count.txt`、`playCount.txt`，以及 IO 示例用的 `a.txt`、`b.txt`、`names.txt`、`students.txt`。`day21/code/demo` 里的 PDF 是 IO 示例。

同一章课件会连续出现在好几天的目录里，每天各有一份 Markdown。

`day02/ASCII码表.md` 里第 44 号沿用了原 Word 的写法（撇号）。标准 ASCII 中 44 是逗号。

<a id="daily"></a>

## 每天学什么

| 天 | 笔记 | 课件 | 这一天的内容 |
| --- | --- | --- | --- |
| <a id="day01"></a>day01 | [总结](<day01/day01总结.md>)、[课堂练习](<day01/课堂练习.md>) | [第一章 Java概述](<day01/第一章_Java概述.md>)、[第二章 基础语法上](<day01/第二章_Java基础语法[上].md>) | 计算机基础、DOS、JDK/JRE/JVM、HelloWorld、环境变量、注释、关键字、标识符 |
| <a id="day02"></a>day02 | [总结](<day02/day02总结.md>)、[课堂练习](<day02/课堂练习.md>) | [第二章 基础语法上](<day02/第二章_Java基础语法[上].md>) | 常量、进制、变量、数据类型、类型转换、运算符。另有 [ASCII码表](<day02/ASCII码表.md>)、[运算符优先级](<day02/Java语言运算符优先级表.md>) |
| <a id="day03"></a>day03 | [总结](<day03/day03总结.md>) | [第二章 基础语法上](<day03/第二章_Java基础语法[上].md>) | 位运算、三目运算、键盘录入、顺序结构、if、switch |
| <a id="day04"></a>day04 | [总结](<day04/code/day04总结.md>)、[自己的总结](<day04/myday04总结.md>) | [第三章 基础语法下](<day04/第三章_Java基础语法[下].md>) | 循环、跳转语句、方法 |
| <a id="day05"></a>day05 | [总结](<day05/day05总结.md>)、[课堂练习](<day05/课堂练习.md>) | [第三章 基础语法下](<day05/第三章_Java基础语法[下].md>) | 方法重载、一维数组、二维数组。另有 [基础知识测试](<day05/Java基础知识测试.md>) |
| <a id="day06"></a>day06 | [总结](<day06/day06总结.md>) | [第四章 面向对象上](<day06/第四章_面向对象[上].md>) | 类与对象、成员、封装、private、this。笔记在 [面向对象思想](<day06/code/01_面向对象思想/面向对象思想.md>)、[类与对象](<day06/code/02_类与对象/类与对象.md>) |
| <a id="day07"></a>day07 | [总结](<day07/day07总结.md>) | [第四章 面向对象上](<day07/第四章_面向对象[上].md>) | 构造方法、static、帮助文档、代码块。另有 [如何使用帮助文档](<day07/code/07_学习并使用帮助文档/如何使用帮助文档.md>) |
| <a id="day08"></a>day08 | [总结](<day08/day08总结.md>) | [第五章 面向对象下](<day08/第五章_面向对象[下].md>) | 继承、方法重写、final、多态。另有 [继承概述](<day08/code/01_继承/继承概述.md>)、[两个面试题](<day08/code/02_方法重写/两个面试题.md>) |
| <a id="day09"></a>day09 | [总结](<day09/day09总结.md>) | [第五章 面向对象下](<day09/第五章_面向对象[下].md>) | 多态、抽象类、接口。另有 [抽象类和接口的区别](<day09/code/05_接口/抽象类和接口的区别.md>) |
| <a id="day10"></a>day10 | [总结](<day10/day10总结.md>) | [第五章 面向对象下](<day10/第五章_面向对象[下].md>) | 形式参数与返回值、包、修饰符、内部类。另有 [常见的修饰符组合](<day10/code/05_常见的修饰符组合/常见的修饰符组合.md>) |
| <a id="day11"></a>day11 | [总结](<day11/day11总结.md>)、[Eclipse的基本使用](<day11/Eclipse的基本使用.md>) | [第六章 Eclipse](<day11/第六章_Eclipse(磨刀不误砍柴工).md>)、[第七章 常用类](<day11/第七章_常用类.md>) | Eclipse、Object |
| <a id="day12"></a>day12 | [总结](<day12/day12总结.md>) | [第七章 常用类](<day12/第七章_常用类.md>) | Scanner、String。另有 [equals 源码笔记](<day12/code/day12_String/itcast_08/String类的equals()方法源码.md>) |
| <a id="day13"></a>day13 | [总结](<day13/day13总结.md>) | [第七章 常用类](<day13/第七章_常用类.md>) | StringBuffer、数组、Arrays、包装类。另有 [Arrays 源码笔记](<day13/code/day13_Array_Arrays/itcast_05/Arrays工具类的源码.md>) |
| <a id="day14"></a>day14 | [总结](<day14/day14总结.md>) | [第七章 常用类](<day14/第七章_常用类.md>) | 正则、Math、Random、System、BigInteger、日期。另有 [正则表达式的规则](<day14/code/day14_Regex/正则表达式的规则.md>) |
| <a id="day15"></a>day15 | [总结](<day15/day15总结.md>) | [第八章 集合](<day15/第八章_集合.md>) | 对象数组、Collection、List。另有 [迭代器源码解析](<day15/code/day15_Collection/itcast_04/迭代器的源码解析.md>) |
| <a id="day16"></a>day16 | [总结](<day16/day16总结.md>)、[练习](<day16/练习.md>) | [第八章 集合](<day16/第八章_集合.md>) | 数据结构、ArrayList/Vector/LinkedList、泛型、JDK5 新特性 |
| <a id="day17"></a>day17 | [总结](<day17/day17总结.md>)、[Collection集合总结](<day17/Collection集合总结.md>) | [第八章 集合](<day17/第八章_集合.md>) | Set，以及 [要练习的代码](<day17/要练习的代码.md>)、[登录注册案例分析](<day17/code/day17_login_regist/登录注册案例分析.md>) |
| <a id="day18"></a>day18 | [总结](<day18/day18总结.md>) | [第八章 集合](<day18/第八章_集合.md>) | Map、Collections |
| <a id="day19"></a>day19 | [File总结](<day19/File总结.md>)、[异常总结](<day19/异常总结.md>) | [第九章 IO流](<day19/第九章_IO流.md>) | File、异常 |
| <a id="day20"></a>day20 | [总结](<day20/day20总结.md>) | [第九章 IO流](<day20/第九章_IO流.md>) | 递归、IO 流分类 |
| <a id="day21"></a>day21 | [总结](<day21/day21总结.md>) | [第九章 IO流](<day21/第九章_IO流.md>) | 缓冲流、转换流、字符流。另有 [day20 课后作业](<day21/code/demo/day20课后作业.md>) |
| <a id="day22"></a>day22 | [总结](<day22/day22总结.md>)、[提纲](<day22/day22.md>) | [第九章 IO流](<day22/第九章_IO流.md>) | 数据流、内存流、打印流、序列化、Properties、NIO |
| <a id="day23"></a>day23 | [总结](<day23/day23总结.md>) | [第十章 多线程](<day23/第十章_多线程.md>) | 多线程 |
| <a id="day24"></a>day24 | [总结](<day24/day24总结.md>) | [第十章 多线程](<day24/第十章_多线程.md>)、[设计原则与设计模式](<day24/扩展知识_面向对象增强(设计原则及常见设计模式).md>) | 多线程、单例模式 |
| <a id="day25"></a>day25 | [总结](<day25/day25总结.md>)、[几句有用的代码](<day25/几句有用的代码.md>) | [第十一章 GUI](<day25/第十一章_GUI(图形界面编程).md>) | 图形界面。另有 [事件监听机制](<day25/code/day25_Frame/itcast_02/事件监听机制.md>)、[登录注册说明](<day25/code/登录注册/登录注册.md>) |
| <a id="day26"></a>day26 | [作业](<day26/homework/day26作业.md>) | 无课件 | 作业要求是把总结补齐。示例在 `day26/resource` 的 Socket 聊天客户端和服务端 |

<a id="review"></a>

## 复习笔记

- [day01review](<复习/day01review.md>)：计算机基础、DOS、JDK、HelloWorld、注释、关键字、标识符
- [day02review](<复习/day02review.md>)：常量、进制、变量、类型转换、运算符
- [day03review](<复习/day03review.md>)：三目运算符
- [day19review](<复习/day19review.md>)：异常、File

<a id="projects"></a>

## 示例工程

每天的 `code` 目录是当天知识点的小例子。每个示例目录里的源码同时写在同目录的 `示例代码.md` 中。成套一点的练习有：

- day17、day25 的登录注册
- day25 的四则运算
- day26 的 Socket 聊天室：`day26/resource/chat_socket_client` 和 `day26/resource/chat_socket_server`
