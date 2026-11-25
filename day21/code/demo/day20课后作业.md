# day20课后作业

> 由 `day21/code/demo/day20课后作业.doc` 转换。

简答题

- 1：递归是什么?注意事项是什么?解决问题的思想是什么?

  - 方法体中调用方法本身的现象。

  - 注意事项：

    - 要有出口

    - 不能次数过多

    - 构造不能递归使用

  - 解决问题的思路：

    - 分解，合并。

    - 找规律和出口。

- 2：IO流的分类?

  - 数据类型：
    - 字节流

      - 字节输入流	InputStream

      - 字节输出流	OutputStream

    - 字符流

      - 字符输入流	Reader

      - 字符输出流	Writer

- 3：如何知道我们到底应该是用字节流还是字符流呢?

  - 如果通过windows记事本打开并能够读懂其中的内容，就使用字符流。否则使用字节流。

- 4：创建字节输出流到底做了哪些事情?

  - 系统创建一个文件

  - 创建一个对象

  - 把对象指向文件

- 5：数据写成功后，为什么要close()?

  - 关闭流对象

  - 释放系统资源

- 6：如何实现数据的换行?

  - 不同的操作系统换行符不一样，

  - windows \r\n

- 7：如何实现数据的追加写入?

  - 构造方法的时候，用第二个参数为true

看方法写中文意思

- FileOutputStream类中的方法：

  - public void write(int b)：一次写一个字节

  - public void write(byte[] b) ：一次写一个字节数组

  - public void write(byte[] b,int off,int len)：：一次写一个字节数组的一部分

FileInputStream类中的方法：

  - public int read()：一次读取一个字节

  - public int read(byte[] b)：一次读取一个字节数组

编程题：(先尝试着自己实现，实在不行，也得照着我的代码敲一遍。)

- 1：递归练习(前两个必须会写代码，后两个最低要求懂思路和看懂代码)

  - A:递归求阶乘

```java
public static int jc(int n) {
if(n==1) {
return 1;
}else {
return n*jc(n-1);
}
}
```

  - B:兔子问题(斐波那契数列)

```java
public static int fib(int n) {
if(n==1 || n==2) {
return 1;
}else {
return fib(n-1)+fib(n-2);
}
}
```

  - C:递归遍历目录下指定后缀名结尾的文件名称

  - D:递归删除带内容的目录

- 2：IO流练习

  - A:把当前项目目录下的a.txt内容复制到当前项目目录下的b.txt中

```java
FileInputStream fis = new FileInputStream("a.txt");
FileOutputStream fos = new FileOutputStream("b.txt");

int by = 0;
while((by=fis.read())!-1) {
fos.write(by);
}

fos.close();
fis.close();
```

  - B:把c:\\a.txt内容复制到d:\\b.txt中

  - C:把e:\\林青霞.jpg内容复制到当前项目目录下的mn.jpg中

```java
FileInputStream fis = new FileInputStream("e:\\林青霞.jpg");
FileOutputStream fos = new FileOutputStream("mn.jpg");

int by = 0;
while((by=fis.read())!-1) {
fos.write(by);
}

fos.close();
fis.close();

FileInputStream fis = new FileInputStream("e:\\林青霞.jpg");
FileOutputStream fos = new FileOutputStream("mn.jpg");

byte[] bys = new byte[1024];
int len = 0;
while((len=fis.read(bys))!=-1) {
fos.write(bys,0,len);
}

fos.close();
fis.close();
```

  - D:把e:\\哥有老婆.mp4复制到当前项目目录下的copy.mp4中
