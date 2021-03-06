# 程序员的数学
- [第1章 0的故事--无即是有](chapter1.md)
- [第2章 逻辑--真与假的二元世界](chapter2.md)
- [第3章 余数--周期性和分组](chapter3.md)
- [第4章 数学归纳法--如何征服无穷数列](chapter4.md)
- [第5章 排列组合--解决计数问题的方法](chapter5.md)
- [第6章 递归--自己定义自己](chapter6.md)
- [第7章 指数爆炸--如何解决复杂问题](chapter7.md)
- [第8章 不可解问题--不可解的数、无法编写的程序](chapter8.md)
- [第9章 什么是程序员数序--总结篇](chapter9.md)

于2017-07-15

## 第1章 0的故事--无即是有
指数法则：  
N<sup>a</sup> * N<sup>b</sup> = N<sup>a+b</sup>  
即“N的a次方乘以N的b次方，等于N的a+b次方”，但N ≠ 0

## 第2章 逻辑--真与假的二元世界
- 真值表
- 文氏图(Venn diagram)  
逻辑关系
 - 非、
 - 和、
 - 或、
 - 异或(exclusive or)  

蕴含:  
如A则B， A => B  

#### 德.摩根定律  
(¬A)∨(¬B) = ¬(A∧B)  
(¬A)∧(¬B) = ¬(A∨B) 

#### 卡诺图（Karnaugh Map）  
将所有命题的真假组合以二维表的形式表示的图。


#### 三值逻辑的德.摩根定律  
(!A) || (!B) = !(A && B)  
(!A) && (!B) = !(A || B)

## 第3章 余数--周期性和分组  
 - 奇偶性(parity)
 - 运用余数，大数字的问题就能简化成小数字的问题。
 - 寻找恋人问题
 - 铺设草席问题
 - 哥尼斯堡七桥问题
 		如果能够一笔画成，必须满足所有定点都是偶点或者只有2个奇数点。 

## 第4章 数学归纳法--如何征服无穷数列
 - 高斯的断言  
 	0到n的整数之和与n*(n+1)/2相等。
  
  
## 第5章 排列组合--解决计数问题的方法
 - 植树问题--不要忘记0
 - 容斥原理（The  principle of Inclusion and Exclusion）  
 	|A∪B| = |A| + |B| - |A∩B|
 - 阶乘(factorial)  
 	n! = n * (n-1) * (n-2) * .... * 3 * 2 * 1
 - 排列(permutation)
   我们将从n张牌中取出k张按一定顺序排列的方法称作**排列**  
	P<sup>k</sup><sub>n</sub> = n * (n-1) * (n-2) * ... * (n-k+1)  
	  = n!/(n-k)!
 - 组合(combination)  
   C<sup>k</sup><sub>n</sub> = P<sup>k</sup><sub>n</sub> /P<sup>k</sup><sub>k</sub>  
	= n!/(n-k)!k!
 	

## 第6章 递归--自己定义自己
 - GNU: GNU is Not Unix
 - 汉诺塔问题  
 	先从小问题着手  
	递推公式：H(n) = H(n-1) + 1 + H(n-1)  (n=0,1,2,3 ...时)
 - 再谈阶乘  
 	定义了 0！= 1
 - 递归(recursive)与归纳(inductive)
 	- 递归： 从一般性前提推出个别性结论
 	- 归纳： 从个别性前提推出一般性结论
 - 斐波那契数列
 - 帕斯卡三角形，又称杨辉三角  
 	C<sub>n</sub><sup>k</sup> = C<sub>n-1</sub><sup>k-1</sup> + C<sub>n-1</sub><sup>k</sup>(0<k<n时)  
    C<sub>n</sub><sup>k</sup> = 1 (n=0或n=k时)
 - 递归图形的例子--谢尔平斯基三角形


## 第7章 指数爆炸--如何解决复杂问题
- 二分查找--利用指数爆炸进行查找
- 用加法实现乘法计算  
	log<sub>n</sub>(A*B) = log<sub>n</sub>A + log<sub>n</sub>B (设 A > 0, B > 0)


## 第8章 不可解问题--不可解的数、无法编写的程序
- 反证法（有时也被称为归谬法）  
	先假设命题的否定形式成立，然后再进行推理，引出矛盾。
- 质数    
	只能被1和本身整除的大于1的整数。  
- 可数  
	集合的元素是有限的，或者集合中的所有元素都与正整数一一对应时，这个集合就被定义为可数（countable）  
- 停机问题  
	判断“某程序在给定数据下，是否会在有限的时间结束运行”的问题。   
- 费马大定理(Fermat's last theorem)  
	当整数n>2时，关于x,y,z的不定方程x<sup>n</sup> + y<sup>n</sup> = z<sup>n</sup>无正数解。  
- 哥德巴赫猜想  
	任意大于3的偶数都可以写成两个质数之和   1+1=2问题

 
## 第9章 什么是程序员数序--总结篇
- 何为解决问题  
	认清模式。进行抽象化






