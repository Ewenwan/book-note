## 第2章 快速开始一个go程序


1. 下划线引入包

	下划线让编译器接受这类导入，并且调用对应包内所有代码文件里定义的init函数。
	init函数会在main函数执行前调用。

	    import (
	    	_ "test"
	    )
 
2. 包级变量：未定义在任何函数作用域内的变量。  
以小写字母开头的标识符是不公开的，不能被其他包中的代码直接访问。
3. 在go语言中，所有变量都被初始化为其零值。  
	- 数值类型：零值是0;
	- 字符串类型：零值是空字符串;
	- 布尔型：零值是false
	- 指针：零值是nil
	- 引用类似：所引用的底层数组结构会被初始化为对应的零值。
	- 被声明为其零值的引用类型的变量，会返回nil作为其值。
	

4. sync.Waitgroup是一个计数信号量，我们可以利用它来统计所有的goroutine是不是都完成了工作。
	
