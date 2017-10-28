# 理解Java #
### 1.字符串不变性 ###

     下面这张图展示了这段代码做了什么

     String s= "abcd";

	 s = s.concat("ef");
	
![](https://i.imgur.com/CsYFPxO.png)

### 2.equals()方法、hashCode()方法的区别 ###

HashCode被设计用来提高性能。equals()方法与hashCode()方法的区别在于：

      1).如果两个对象相等(equal)，那么他们一定有相同的哈希值。
      2).如果两个对象的哈希值相同，但他们未必相等(equal)。

![](https://i.imgur.com/FCrTDAR.png)

### 3.Java异常类的层次结构 ###

图中红色部分为受检查异常。它们必须被捕获，或者在函数中声明为抛出该异常。
![](https://i.imgur.com/YzDb2cr.png)

### 4.集合类的层次结构 ###

注意Collections和Collection的区别。（*Collections包含有各种有关集合操作的静态多态方法*）

![](https://i.imgur.com/nT7p9Yq.png)

### 5.Java的同步 ###

Java的同步机制类比于建筑物来阐明:

![](https://i.imgur.com/AUJFIav.png)

### 6.别名 ###

别名意味着有多个变量指向同一可被更新的内存块，这些别名分别是不同的对象类型。

![](https://i.imgur.com/Zq9Xo8m.png)

### 7.堆和栈 ###

图解表明了方法和对象在运行时内存中的位置:

![](https://i.imgur.com/iInOzmS.png)

### 8.Java虚拟机运行时的数据区域

![](https://i.imgur.com/Y5DN9Ll.png)