## OI 中常用的几类距离 ：

### 曼哈顿距离

对于平面上两点 $A(x_1, y_1)$, $B(x_2, y_2)$ $Dis(A, B) = |x_1-x_2| + |y_1-y_2|$

一般来讲，我们只会用到二维平面上的曼哈顿距离

### 切比雪夫距离

对于平面上两点 $A(x_1, y_1)$, $B(x_2, y_2)$ $Dis(A, B) = \max(|x_1-x_2| , |y_1-y_2|)$

对于两个 $n$ 维向量 $\vec A(x_{11}, x_{12}, \cdots,x_{1n})$  $\vec B(x_{21}, x_{22}, \cdots,x_{2n})$

$Dis(A, B) = \max\limits_i(|x_{1i}-x_{2i}|)$

### 欧几里得距离 （又称欧氏距离）

欧几里得距离是两点的直线距离。

对于平面上两点 $A(x_1, y_1)$, $B(x_2, y_2)$ $Dis(A, B) = \sqrt{(x_1-x2)^2+(y1-y2)^2}$

对于两个 $n$ 维向量 $\vec A(x_{11}, x_{12}, \cdots,x_{1n})$  $\vec B(x_{21}, x_{22}, \cdots,x_{2n})$

$Dis(A, B) = \sqrt{\sum\limits_{k=1}^n(x_{1k}-x_{2k})^2}$

### L_m 距离

一般地，我们定义平面上两点 $A(x_1, y_1)$, $B(x_2, y_2)$ 之间的 $L_m$ 距离为

$dist~L_m = (|x_1-x_2|^m+|y1-y2|^m)^{\frac{1}{m}}$

特殊的， $L_2$ 距离就是欧几里得距离， $L_1$ 距离就是曼哈顿距离。

### 汉明距离

汉明距离是两个字符串之间的距离，它表示两个长度相同的字符串对应位字符不同的数量

我们可以简单的认为对两个串进行异或运算， 结果为 1 的数量就是两个串的汉明距离。

* * *

当然， 还有其他的一些距离，但是在 OI 中并不常用，有兴趣的话可以了解一下。