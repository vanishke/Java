# Java基础知识测试

> 由 `day05/Java基础知识测试.doc` 转换。

单选题：（每道题目2分）

1.	下列哪个声明是错误的？（）

A.  int  i=10;

B.  float  f=1.1;

C.  double  d=34.4;

D.  byte  b=127;

变量的定义

数据类型

2.	下面哪个不是java中的关键字？（）

A.	public

B.  true

C.  main

D.  class

关键字

3.	下面程序哪个语句是正确的

A.  byte  a=0,b=3; byte c =a+b;

B.  short  s =23; s=s+12;

C.  short  s=23; s+=12;

D.  float  f = 23+23.23;

类型转换

运算符

4.	下面程序执行的结果是？()

```java
class  Test
{
public  static  void  main(String[] args)
{
System.out.println(“”+‘a’+1);
}
}
```

A.	98

B.  a1

C.  971

D.  197

字符串的连接

5.	下面程序执行的结果是？（）

```java
int i = 100;
while(true)
{
if (i++ > 100)
{
break;
}
System.out.println(i);
}
```

A.  100

B.  101

C.  102

D.  报错

判断语句

循环语句

控制跳转语句

6.  下面程序的运行结果是    (  )

```java
int a=3, b=1;
if(a==b)
{
System.out.println("a="+a);
}
```

A.  a=1

B.  a=3

C.  编译错误

D.  正常运行但没有输出

判断语句

7.	下面程序的运行后,结果正确的是：

```java
int a=1,b=2;
```

int c=(a+b>3?a++:++b); a=1,b=3,c=3

A.  a=2,b=3

B.  a=1,b=3

C.  a=1,b=2

D.  c=2

8.	下面程序的运行结果

```java
class Demo
{
public static int fun(int c)
{
return  c+=2;
}
public static void main(String[] args)
{
int temp = fun(2);
System.out.println(temp);
}
}
```

A.  2

B.  4

C.  6

D.  8

方法调用

9.	下面数组定义错误的是（）

```java
A.  int [] arr ={23,45,65,78,89};
```

B.  int [] arr=new int[10] ;

```java
C.  int [] arr=new int[4]{3,4,5,6};
```

D.  int [] arr={‘a’, 23 , 45 , 6}；

数组定义

10. 下面程序执行的结果是？（ ）

```java
int x =1,y=1;
if(x++==2 & ++y==2)
{
x=7;
}
System.out.println("x="+x+"  ,  y="+y);
```

A.  x=1  y=2

B.  x=7  y=1

C.  x=7  y=2

D.  x=2  y=2

运算符

判断语句

11. 下面不属于基本数据类型的是（）

A.  int

B.  double

C.  long

D.  int[]

数据类型

12. 下面程序执行的结果是？（ ）

```java
boolean b=true;
if(b=false)
{
System.out.println("a");
}
else if(b)
{
System.out.println("b");
}
else if(!b)
{
System.out.println("c");
}
else
{
System.out.println("d");
}
```

A.	a

B.	b

C.	c

D.	d

13. 下面程序执行的结果是？（）

```java
int x=2,y=3;
switch(x)
{
```

- default:

```java
y++;
case 3:
y++;
case 4:
y++;
}
Sysetem.out.println("y="+y);
```

A.  3

B.  4

C.  5

D.  6

switch的执行流程

14. 下面程序执行的结果

```java
for(int  i=1;i<=10;i++)
{
if (i%3==0)
{
continue;
}
System.out.println(“java基础班”);
}
```

在屏幕上打印几次“java基础班”?(  )

A.  5

B.  6

C.  7

D.  8

15.阅读下面代码段：

```java
class Demo
{
public static void main (String[] args)
{
int[] arr = new int[10];
System.out.println(arr[1]);
}
}
```

执行结果正确的说法是(  )

A.  编译时将产生错误

B.  编译时正确，运行时将产生错误

C.  输出零

D.  输出空

16 .和下面代码能完成相同的选项是（）

```java
int i=1;
int sum=0;
while(i<=100)
{
if(i%2==0)
{
sum=sum+i;
}
i++;
}

A.  for (int x =1; x<=100;x++){ sum=sum+x;}
B.  for (int x =0; x<=100;x+=2){ sum=sum+x;}
C.  for (int x =1; x<=100;x+=2){ sum=sum+x;}
```

D.上述全对

17.  以下代码输出是（  ）

```java
int i=0;
int sum=0;
while(i<=10)
{
i++;
if( i%2 !=0 )
continue;
sum+=i;

}
System.out.println(sum);
```

A.  55

B.  45

C.  35

D.  30

18.  给出下列代码片段:

```java
if ( x > 0 ) { System.out.println(“Hello”); }
else if ( x >-3 ) { System.out.pirntln ( “I am Tom”); }
else { System.out.println (“How are you?”); }
```

请问将打印字符串 “How are you ?”的x的范围是（ ）

A.   x>0

B.   x > -3

C.   x <= -3

D.   x <=0 & x >-3

19． 下列代码执行的结果为( )

```java
class Demo
{
public static void main(String[] args)
{
int num = max(43,34);
System.out.println(num);
}

public static int max(int a,int b)
{
return a>b?a:b;

}
}
```

A.  43

B.  23

C.  77

D.  9

20 .下面程序执行的结果是( )

```java
class Demo
{
public static void main(String [] args)
{
int a=10;
if(a++>10)
{
a=20;
}
System.out.println(a);
```

}
}

A.  11

B.  12

C.  20

D.  21

多选题：（每道题目3分）

21. 下面哪些是合法的标志符（）

A.  2variable

B.  variable2

C.  what$

D.  _3_

22.	下列函数中能和函数int max(int  a,  int  b, double  c)构成重载关系的是(  )

A.  double  max(int  a, int  b, double  c)

B.  void  max(int  a, double  c, int  b)

C.  int  max(double a, int  b)

D.  int  max(int  x, int  y, double  z)

23. 下面的说法正确的是(  )

A.  byte ,short,char 数据类型可以自动转化为int

B.  float 数据类型可以自动转换为long。

C.  在java语言中默认小数为double

D.  byte a=23;  byte b=12;  a+b的结果为byte类型

24. 下面关于函数描述正确的是（）

A.  函数是对功能代码块的封装

B.  函数没有返回值的时候什么都不用写

C.  没有返回值的函数，不能有return 语句

D.  函数是可以没有形参的

25. 下面关于循环描述正确的是（）

A.  while循环先判断循环条件，后执行循环操作

B.  while 至少会执行一次

C.  do-while先进行循环条件判断，后执行循环操作

D.  do-while循环至少执行一次，后进行循环判断

简答题目：(每道题目5分）

26：JDK,JRE,JVM是什么，有什么用，它们之间又有什么关系?

- JDK:开发工具	包括JRE+tools

- JRE:运行环境	包括JVM+核心类库

- JVM:保证java语言跨平台

27：数组是基本类型吗? Java中基本数据类型分类有哪些?

- 不是。

- 4类8种。

- 整数：byte,short,int,long

- 浮点数：float,double

- 字符：char

- 布尔：boolean

28：函数是什么?它的运行特点是什么?

- 完成特定功能的代码块。

- 不调用不执行。

29：数组是什么?我们根据什么可以获取数组中的元素呢?

- 数组是存储同一种数据类型的多个元素的集合。

- 索引。

30：请说说什么时候使用变量，什么时候使用if语句，什么时候使用循环语句?说的有理即可得分。

- 如何数据是变化的，就需要使用变量。

- 如果要进行判断，就使用if语句。

- 如果要多次做某件事情，可以使用循环。

编程题目：(总共20分,分配6,7,7）

注意：命名规范

31：在main方法中写一段代码，实现在控制台输出九九乘法表。

32：请写一个方法sum，实现求两个数之和。要求在main中调用。

33：请写一个方法printArray,实现遍历整数数组。要求在main中调用。
