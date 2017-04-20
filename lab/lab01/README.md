实验一，JDK, Compiling, Javadoc, Eclipse, Strings
======

### 介绍

本实验的目标是让你熟悉使用Eclipse，Java编译器，Javadoc。 本实验花费时间不多，后续实验将需花费更多时间。

### 目标

完成本实验后，你将能够：
- 安装Java 8和Eclipse
- 在Eclipse中编译和执行一个Java程序
- 应用基本的String处理方法来解析和创建字符串
- 创建一个类并构造该类的实例
- 使用Javadoc来为代码生成文档

### 实验步骤
1. 如你未完成如下安装则请按指示安装
  - 下载并安装[JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
  - 本课程要求Java 7或以上版本，可以控制台输入`java -version`来检查你的Java版本
  - 下载并安装最新版本的[Eclipse IDE for Java Developers(Eclipse Classic也行)](http://www.eclipse.org/downloads/)。如果你已经安装Eclipse版本3，建议升级到版本4。

2. 在Eclipse中，创建一个称为`lab1`的新项目：
  选择 *File/New Java Project* 
  或者
  选择 *File/New Project/Java Project*

3. 在该项目中，创建一个称为**Driver**的类
  - 在*Package Explorer*中选择lab1项目
  - 右击后选择*New/Class*
  - 给一个类名(**Driver**)，然后点*Finish*

4. 任务1：在你的**Driver**类中，创建一个**main**方法。 **main**方法应该在屏幕上输出*Hello world!*。

5. 编译和执行你的程序。 点击顶部工具条上的绿色*Start*按钮。 你应该看到结果字符串被显示在你的控制台窗口中。任务1完成。

6. 任务2：创建一个称为**Planning**的类。 该类表示一门课程的登记信息。 该类必须具备如下属性：
  - 必须有一个内部字符串数组，长度是4，称为*info*。
  - 必须有一个构造函数：
  ```code
    public Planning(String input)
  ```
  上面的input是s1,s2,s3形式的字符串，其中 
    - s1表示只包含字母数字的字符串
    - s1,s2表示只包含数字字符的字符串（不含空格）
   例如，*Java,153,50*表示满足条件的一个字符串，其中*s1 = Java*，*s2 = 153*，*s3 = 50*. 在程序中，我们将*s1*解释为课程名，*s2*解释为课程登记数，*s3*解释为最大课程人数。
   该方法将*s1*以全部大写方式存入**info[0]**，将*s2*存入**info[1]**，将*s3*存入**info[2]**，并将*(s2 + s3 - 1)/s3*，所需的课程节数，存入**info[3]**。注意最后一个操作需要做类型转换。
  - 我们


 