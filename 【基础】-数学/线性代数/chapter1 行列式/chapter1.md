## 二阶与三阶行列式

### 二元线性方程组与二阶行列式

解二元线性方程组 $\longrightarrow$ 二阶行列式
$$
\left\{\begin{array}{l}
a_{11} x_1+a_{12} x_2=b_1, \\
a_{21} x_1+a_{22} x_2=b_2 .
\end{array}\right.
$$

- ${b_1}$和${b_2}$：常数
- ${a_{ij}}$：第$i$个方程的第$j$个未知数$x_j$的系数

两个方程两端同时乘以$a_{22}$和$a_{12}$
$$
\left\{\begin{array}{l}
a_{22}\left(a_{11} x_1+a_{12} x_2\right)=a_{22} b_1 \\
a_{12}\left(a_{21} x_1+a_{22} x_2\right)=a_{12} b_2
\end{array}\right.
$$
两式相减
$$
\left(a_{11} a_{22}-a_{12} a_{21}\right) x_1=b_1 a_{22}-a_{12} b_2
$$
两个方程两端同时乘以$a_{21}$和$a_{11}$
$$
\left\{\begin{array}{l}
a_{21}\left(a_{11} x_1+a_{12} x_2\right)=a_{21} b_1 \\
a_{11}\left(a_{21} x_1+a_{22} x_2\right)=a_{11} b_2
\end{array}\right.
$$
两式相减
$$
\left(a_{11} a_{22}-a_{12} a_{21}\right) x_2=a_{11} b_2-b_1 a_{21}
$$
如果$a_{11} a_{22}-a_{12} a_{21}\neq0$，可以解出：
$$
x_1=\frac{b_1 a_{22}-a_{12} b_2}{a_{11} a_{22}-a_{12} a_{21}} \quad x_2=\frac{a_{11} b_2-b_1 a_{21}}{a_{11} a_{22}-a_{12} a_{21}}
$$

------

**数表**：
$$
\begin{array}{ll}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{array}
$$
**表达式**：$a_{11} a_{22}-a_{12} a_{21}$

**二阶行列式**：$\left|\begin{array}{ll}a_{11} & a_{12} \\ a_{21} & a_{22}\end{array}\right|$

- $a_{ij}$：元素/元
- $i$：行标
- $j$：列标
- $(i,j)$元：位于第$i$行第$j$列的元素
- 主对角线/副对角线

------

利用二阶行列式，式子简记为：
$$
b_1 a_{22}-a_{12} b_2=\left|\begin{array}{ll}
b_1 & a_{12} \\
b_2 & a_{22}
\end{array}\right|, \quad a_{11} b_2-b_1 a_{21}=\left|\begin{array}{ll}
a_{11} & b_1 \\
a_{21} & b_2
\end{array}\right| .
$$
若记
$$
D=\left|\begin{array}{ll}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{array}\right|, \quad D_1=\left|\begin{array}{ll}
b_1 & a_{12} \\
b_2 & a_{22}
\end{array}\right|, \quad D_2=\left|\begin{array}{ll}
a_{11} & b_1 \\
a_{21} & b_2
\end{array}\right|,
$$
利用二阶行列式的概念，改写$x_1$，$x_2$的表示：
$$
x_1=\frac{D_1}{D}=\frac{\left|\begin{array}{ll}
b_1 & a_{12} \\
b_2 & a_{22}
\end{array}\right|}{\left|\begin{array}{ll}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{array}\right|}, \quad x_2=\frac{D_2}{D}=\frac{\left|\begin{array}{ll}
a_{11} & b_1 \\
a_{21} & b_2
\end{array}\right|}{\left|\begin{array}{ll}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{array}\right|} .
$$

- $D$：系数行列式

### 三阶行列式

解三元线性方程组 $\longrightarrow$ 三阶行列式
$$
\left\{\begin{array}{l}
a_{11} x_1+a_{12} x_2+a_{13} x_3=b_1 \\
a_{21} x_1+a_{22} x_2+a_{23} x_3=b_2 \\
a_{31} x_1+a_{32} x_2+a_{33} x_3=b_3
\end{array}\right.
$$

- ${b_1}$、${b_2}$和${b_3}$：常数
- ${a_{ij}}$：第$i$个方程的第$j$个未知数$x_j$的系数

后两个方程两端同时乘以$a_{33}$和$a_{22}$
$$
\left\{\begin{array}{l}
a_{33}\left(a_{21} x_1+a_{22} x_2+a_{23} x_3\right)=a_{33} b_2 \\
a_{23}\left(a_{31} x_1+a_{32} x_2+a_{33} x_3\right)=a_{23} b_3
\end{array}\right.
$$
两式相减
$$
\left(a_{21} a_{33}-a_{23} a_{31}\right) x_1+\left(a_{22} a_{33}-a_{23} a_{32}\right) x_2=b_2 a_{33}-a_{23} b_3
$$
后两个方程两端同时乘以$a_{32}$和$a_{22}$
$$
\left\{\begin{array}{l}
a_{32}\left(a_{21} x_1+a_{22} x_2+a_{23} x_3\right)=a_{32} b_2 \\
a_{22}\left(a_{31} x_1+a_{32} x_2+a_{33} x_3\right)=a_{22} b_3
\end{array}\right.
$$
两式相减
$$
\left(a_{21} a_{32}-a_{22} a_{31}\right) x_1+\left(a_{23} a_{32}-a_{22} a_{33}\right) x_3=b_2 a_{32}-a_{22} b_3
$$
目前得到有方程（1）（2）
$$
\begin{aligned}
&\left(a_{21} a_{33}-a_{23} a_{31}\right) x_1+\left(a_{22} a_{33}-a_{23} a_{32}\right) x_2=b_2 a_{33}-a_{23} b_3 \\
&\left(a_{21} a_{32}-a_{22} a_{31}\right) x_1+\left(a_{23} a_{32}-a_{22} a_{33}\right) x_3=b_2 a_{32}-a_{22} b_3
\end{aligned}
$$
原方程组的第一个方程同时乘以$a_{22} a_{33}-a_{23} a_{32}$，得到方程（3）’
$$
\begin{aligned}
&\left(a_{11} a_{22} a_{33}-a_{11} a_{23} a_{32}\right) x_1+\left(a_{12} a_{22} a_{33}-a_{12} a_{23} a_{32}\right) x_2+\left(a_{13} a_{22} a_{33}-a_{13} a_{23} a_{32}\right) x_3=b_1 a_{22} a_{33}-b_1 a_{23} a_{32}
\end{aligned}
$$
方程（1）两端乘以${-a_{12}}$，得到方程（1）‘
$$
\begin{aligned}
\left(a_{12} a_{23} a_{31}-a_{12} a_{21} a_{33}\right) x_1 &+\left(a_{12} a_{23} a_{32}-a_{12} a_{22} a_{33}\right) x_2=a_{12} a_{23} b_3-a_{12} b_2 a_{33}
\end{aligned}
$$
方程（2）两端乘以${a_{13}}$，得到方程（2）‘
$$
\begin{aligned}
\left(a_{13} a_{21} a_{32}-a_{13} a_{22} a_{31}\right) x_1 &+\left(a_{13} a_{23} a_{32}-a_{13} a_{22} a_{33}\right) x_3 a_{13} b_2 a_{32}-a_{13} a_{22} b_3
\end{aligned}
$$
联立方程（1）‘、（2）‘、（3）‘
$$
\begin{aligned}
&\left(a_{11} a_{22} a_{33}-a_{11} a_{23} a_{32}\right) x_1+\left(a_{12} a_{22} a_{33}-a_{12} a_{23} a_{32}\right) x_2+\left(a_{13} a_{22} a_{33}-a_{13} a_{23} a_{32}\right) x_3=b_1 a_{22} a_{33}-b_1 a_{23} a_{32} \\
&\begin{aligned}
\left(a_{12} a_{23} a_{31}-a_{12} a_{21} a_{33}\right) x_1 &+\left(a_{12} a_{23} a_{32}-a_{12} a_{22} a_{33}\right) x_2=a_{12} a_{23} b_3-a_{12} b_2 a_{33} \\
\left(a_{13} a_{21} a_{32}-a_{13} a_{22} a_{31}\right) x_1 &+\left(a_{13} a_{23} a_{32}-a_{13} a_{22} a_{33}\right) x_3=a_{13} b_2 a_{32}-a_{13} a_{22} b_3
\end{aligned}
\end{aligned}
$$
三式相加，得到
$$
\begin{aligned}
&\left(a_{11} a_{22} a_{33}+a_{12} a_{23} a_{31}+a_{13} a_{21} a_{32}\right. \left.-a_{11} a_{23} a_{32}-a_{12} a_{21} a_{33}-a_{13} a_{22} a_{31}\right) x_1 \\
&=b_1 a_{22} a_{33}+a_{12} a_{23} b_3+a_{13} b_2 a_{32}-a_{13} a_{22} b_3-a_{12} b_2 a_{33}-b_1 a_{23} a_{32}
\end{aligned}
$$
$\color{red}{不方便记忆，因此引入三阶行列式}$

------

**数表**：
$$
\begin{array}{lll}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{array}
$$
**表达式**：$a_{11} a_{22} a_{33}+a_{12} a_{23} a_{31}+a_{13} a_{21} a_{32}-a_{11} a_{23} a_{32}-a_{12} a_{21} a_{33}-a_{13} a_{22} a_{31}$

**三阶行列式**：$\left|\begin{array}{lll}a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33}\end{array}\right|$

------

利用三阶行列式，等式简记为：
$$
\left|\begin{array}{lll}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{array}\right| x_1=\left|\begin{array}{lll}
b_1 & a_{12} & a_{13} \\
b_2 & a_{22} & a_{23} \\
b_3 & a_{32} & a_{33}
\end{array}\right|
$$
同理得到
$$
\left|\begin{array}{lll}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{array}\right| x_2=\left|\begin{array}{lll}
a_{11} & b_1 & a_{13} \\
a_{21} & b_2 & a_{23} \\
a_{31} & b_3 & a_{33}
\end{array}\right|
$$

$$
\left|\begin{array}{lll}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{array}\right| x_3=\left|\begin{array}{lll}
a_{11} & a_{12} & b_1 \\
a_{21} & a_{22} & b_2 \\
a_{31} & a_{32} & b_3
\end{array}\right|
$$

若记
$$
D=\left|\begin{array}{ll}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{array}\right|, \quad D_1=\left|\begin{array}{ll}
b_1 & a_{12} & a_{13} \\
b_2 & a_{22} & a_{23} \\
b_3 & a_{32} & a_{33}
\end{array}\right|, \quad D_2=\left|\begin{array}{ll}
a_{11} & b_1 & a_{13} \\
a_{21} & b_2 & a_{23} \\
a_{31} & b_3 & a_{33}
\end{array}\right|, \quad D_3=\left|\begin{array}{ll}
a_{11} & a_{12} & b_1 \\
a_{21} & a_{22} & b_2 \\
a_{31} & a_{32} & b_3
\end{array}\right|,
$$
利用三阶行列式的概念，改写$x_1$，$x_2$，$x_3$的表示：
$$
x_1=\frac{D_1}{D}, x_2=\frac{D_2}{D}, x_3=\frac{D_3}{D}
$$

- $D$：系数行列式

------

$\color{green}{行列式按一行展开}$：这里举例按照第一行展开
$$
\left|\begin{array}{lll}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{array}\right|=a_{11}\left|\begin{array}{ll}
a_{22} & a_{23} \\
a_{32} & a_{33}
\end{array}\right|-a_{12}\left|\begin{array}{ll}
a_{21} & a_{23} \\
a_{31} & a_{33}
\end{array}\right|+a_{13}\left|\begin{array}{ll}
a_{21} & a_{22} \\
a_{31} & a_{32}
\end{array}\right|
$$
再进行拓展

在空间解析几何中

- 向量积

$\mathbf{a}=a_1 \mathbf{i}+a_2 \mathbf{j}+a_3 \mathbf{k} \quad \mathbf{b}=b_1 \mathbf{i}+b_2 \mathbf{j}+b_3 \mathbf{k}$
$$
\begin{aligned}
\mathbf{a} \times \mathbf{b}=\left|\begin{array}{ccc}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3
\end{array}\right| &=\left|\begin{array}{cc}
a_2 & a_3 \\
b_2 & b_3
\end{array}\right| \mathbf{i}-\left|\begin{array}{cc}
a_1 & a_3 \\
b_1 & b_3
\end{array}\right| \mathbf{j}+\left|\begin{array}{cc}
a_1 & a_2 \\
b_1 & b_2
\end{array}\right| \mathbf{k}
\end{aligned}
$$

$$
\mathbf{a} \times \mathbf{b}=\left|\begin{array}{ll}
a_2 & a_3 \\
b_2 & b_3
\end{array}\right| \mathbf{i}+\left|\begin{array}{ll}
a_3 & a_1 \\
b_3 & b_1
\end{array}\right| \mathbf{j}+\left|\begin{array}{cc}
a_1 & a_2 \\
b_1 & b_2
\end{array}\right| \mathbf{k}
$$

$$
\mathbf{a} \times \mathbf{b}=\left\{\left|\begin{array}{ll}
a_2 & a_3 \\
b_2 & b_3
\end{array}\right|,\left|\begin{array}{ll}
a_3 & a_1 \\
b_3 & b_1
\end{array}\right|,\left|\begin{array}{ll}
a_1 & a_2 \\
b_1 & b_2
\end{array}\right|\right\}
$$

> 以上三种表示方式都是正确的

- 混合积

$\mathbf{a}=a_1 \mathbf{i}+a_2 \mathbf{j}+a_3 \mathbf{k}=\left\{a_1, a_2, a_3\right\}$
$\mathbf{b}=b_1 \mathbf{i}+b_2 \mathbf{j}+b_3 \mathbf{k}=\left\{b_1, b_2, b_3\right\}$
$\mathbf{c}=c_1 \mathbf{i}+c_2 \mathbf{j}+c_3 \mathbf{k}=\left\{c_1, c_2, c_3\right\}$

$\mathbf{b} \times \mathbf{c}=\left\{\left|\begin{array}{ll}b_2 & b_3 \\ c_2 & c_3\end{array}\right|,\left|\begin{array}{ll}b_3 & b_1 \\ c_3 & c_1\end{array}\right|,\left|\begin{array}{ll}b_1 & b_2 \\ c_1 & c_2\end{array}\right|\right\}$
$$
\begin{aligned}
&[\mathbf{a} \mathbf{b} \mathbf{c}]=\mathbf{a} \cdot(\mathbf{b} \times \mathbf{c})\\
&=\left\{a_1, a_2, a_3\right\} \cdot\left\{\left|\begin{array}{ll}
b_2 & b_3 \\
c_2 & c_3
\end{array}\right|,\left|\begin{array}{cc}
b_3 & b_1 \\
c_3 & c_1
\end{array}\right|,\left|\begin{array}{cc}
b_1 & b_2 \\
c_1 & c_2
\end{array}\right|\right\}\\
&=a_1\left|\begin{array}{ll}
b_2 & b_3 \\
c_2 & c_3
\end{array}\right|+a_2\left|\begin{array}{ll}
b_3 & b_1 \\
c_3 & c_1
\end{array}\right|+a_3\left|\begin{array}{ll}
b_1 & b_2 \\
c_1 & c_2
\end{array}\right|\\
&=\left|\begin{array}{lll}
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3 \\
c_1 & c_2 & c_3
\end{array}\right|
\end{aligned}
$$

## 全排列和对换

### 排列及其逆序数

**全排列（排列）**：把$n$个不同的元素排成一列

**逆序**：对于$n$个不同的元素,先规定各元素之间有一个标准次序（例如$n$个不同的自然数，可规定由小到大为标准次序），于是在这$n$个元素的任一排列中，当某一对元素的先后次序与标准次序不同时，就说它构成$1$个逆序。

**逆序数**：一个排列中所有逆序的总数。

逆序数为奇数的排列叫做**奇排列**，逆序数为偶数的排列叫做**偶排列**。

$\color{red}{计算排序的逆序数的方法}$

不失一般性，不妨设$n$个元素为$1$至$n$这$n$个自然数，并规定由小到大为标准次序。设$p_1p_2...p_n$为这$n$个自然数的一个排列，考虑元素$p_i$（$i= 1 ,2 ,… , n$ ） ，如果比$p_i$大的且排在$p_i$前面的元素有$t_i$个，就说$p_i$这个元素的逆序数是$t_i$。

排列的逆序数=全体元素的逆序数之总和$t=t_1+t_2+\cdots+t_n=\sum_{i=1}^n t_i$

### 对换

**对换**：在排列中，将任意两个元素对调，其余元素不动。

【定理】==一个排列中的任意两个元素兑换，排列改变奇偶性。==

证明：

$a_1 \cdots a_l a b b_1 \cdots b_m$

- 相邻对换 $a_1 \cdots a_l a b b_1 \cdots b_m \longrightarrow a_1 \cdots a_l b a b_1 \cdots b_m$
  - $a<b$：$a$的逆序数增加$1$而$b$的逆序数不变
  - $a>b$：$a$的逆序数不变而$b$的逆序数增加$1$
- 一般对换 $a_1 \cdots a_l a b_1 \cdots b_m b c_1 \cdots c_n \longrightarrow a_1 \cdots a_l b b_1 \cdots b_m a c_1 \cdots c_n$
  1. $a_1 \cdots a_l a b_1 \cdots b_m b c_1 \cdots c_n \longrightarrow a_1 \cdots a_l a b b_1 \cdots b_m c_1 \cdots c_n$：$m$次对换
  2. $a_1 \cdots a_l a b b_1 \cdots b_m c_1 \cdots c_n \longrightarrow a_1 \cdots a_l b b_1 \cdots b_m a c_1 \cdots c_n$ ：$m+1$次对换

累计$2m+1$次相邻对换，奇偶性发生变换。

### n 阶行列式的定义

回忆三阶行列式

$\begin{aligned} &\left|\begin{array}{lll}a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33}\end{array}\right| \\=& a_{11} a_{22} a_{33}+a_{12} a_{23} a_{31}+a_{13} a_{21} a_{32}-a_{11} a_{23} a_{32}-a_{12} a_{21} a_{33}-a_{13} a_{22} a_{31} . \end{aligned}$

任意一项表示为：$a_{1p_1}a_{2p_2}a_{3p_3}$

$(p_1,p_2,p_3)=\{(1,2,3),(2,3,1),(3,1,2),(1,3,2),(2,1,3),(3,2,1)\}$

带正号的三项列标排列是123，231，312；（偶排列）

带负号的三项列标排列是132，213，321。（奇排列）

<u>各项的正负号表示$(-1)^t$（$t$为列标排序的逆序数）</u>

因此改写三阶行列式

$\left|\begin{array}{lll}a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33}\end{array}\right|=\sum(-1)^t a_{1 p_1} a_{2 p_2} a_{3 p_3}$

------

**$n$阶行列式**：
$$
\begin{array}{cccc}
a_{11} & a_{12} & \cdots & a_{1 n} \\
a_{21} & a_{22} & \cdots & a_{2 n} \\
& \cdots  \cdots & \cdots & \\
a_{n 1} & a_{n 2} & \cdots & a_{n n}
\end{array}
$$
自由组合不同行不同列的$n$个数的乘积，并冠以符号$(-1)^t$并求代数和，得到$n$阶行列式。

按照<u>行顺序</u>：
$$
\left|\begin{array}{llll}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\ldots & \ldots & \ldots & \ldots \\
a_{n 1} & a_{n 2} & \ldots & a_{n n}
\end{array}\right|=\sum_{p_1, p_2, \ldots, p_n}(-1)^{t} a_{1 p_1} a_{2 p_2} \cdots a_{n p_n}
$$
按照<u>列顺序</u>：
$$
\left|\begin{array}{llll}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\ldots & \ldots & \ldots & \ldots \\
a_{n 1} & a_{n 2} & \ldots & a_{n n}
\end{array}\right|=\sum_{p_1, p_2, \ldots, p_n}(-1)^{t} a_{p_1 1} a_{p_2 2} \cdots a_{p_n n}
$$
任意顺序：
$$
\left|\begin{array}{llll}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\ldots & \ldots & \ldots & \ldots \\
a_{n 1} & a_{n 2} & \ldots & a_{n n}
\end{array}\right|=\sum(-1)^{t(r_1...r_n)+t(s_1...s_n)} a_{r_1 s_1} a_{r_2 s_2} \cdots a_{r_n s_n}
$$
记作$det(a_{ij})$

注：当$n=1$，一阶行列式$|a|=a$

------

**下三角行列式**（斜边为主对角线，上角均为0）：
$$
D=\left|\begin{array}{cccc}
a_{11} & & & \\
a_{21} & a_{22} & & 0 \\
\vdots & \vdots & \ddots & \\
a_{n 1} & a_{n 2} & \cdots & a_{n n}
\end{array}\right|=a_{11} a_{22} \cdots a_{n n}
$$

> 同理还有上三角行列式（斜边为主对角线，下角均为0）

下三角行列式（斜边为次对角线，上角为0）：$D=(-1)^{\frac{n(n-1)}{2}} a_{1 n} a_{2 n-1} \cdots a_{n 1}$

> 同理还有下三角行列式（斜边为次对角线，下角为0）

【推论】==对角行列式==（斜边为主对角线）
$$
\left|\begin{array}{llll}
\lambda_1 & & & \\
& \lambda_2 & & \\
& & \ddots & \\
& & & \lambda_n
\end{array}\right|=\lambda_1 \lambda_2 \cdots \lambda \text {, }
$$

> 同理还有对角行列式（斜边为次对角线）

## 行列式的性质

【性质】==1. 行列式与它的转置行列式相等。==

【性质】==2. 对换行列式的两行（列），行列式变号。==

【推论】==如果行列式有两行(列)完全相同,则此行列式等于零。==

【性质】==3. 行列式的某一行（列）中所有的元素都乘以同一数$k$，等于用数k乘此行列式。==

【推论】==行列式中某一行（列）的所有元素的公因子可以提到行列式记号外面。==

【性质】==4. 行列式中如果有两行（列）元素成比例，则此行列式等于零。==

【性质】==5. 若行列式的某一行（列）的元素都是两数之和，例如第$i$行的元素都是两数之和：==
$$
D=\left|\begin{array}{cccc}
a_{11} & a_{12} & \cdots & a_{1 n} \\
\vdots & \vdots & & \vdots \\
a_{i 1}+a_{i 1}^{\prime} & a_{i 2}+a_{i 2}^{\prime} & \cdots & a_{i n}+a_{i n}^{\prime} \\
\vdots & \vdots & & \vdots \\
a_{n 1} & a_{n 2} & \cdots & a_{n n}
\end{array}\right|
$$
==则$D$等于下列两个行列式之和：==
$$
D=\left|\begin{array}{cccc}
a_{11} & a_{12} & \cdots & a_{1 n} \\
\vdots & \vdots & & \vdots \\
a_{i 1} & a_{i 2} & \cdots & a_{i n} \\
\vdots & \vdots & & \vdots \\
a_{n 1} & a_{n 2} & \cdots & a_{n n}
\end{array}\right|+\left|\begin{array}{cccc}
a_{11} & a_{12} & \cdots & a_{1 n} \\
\vdots & \vdots & & \vdots \\
a_{i 1}^{\prime} & a_{i 2}^{\prime} & \cdots & a_{i n}^{\prime} \\
\vdots & \vdots & & \vdots \\
a_{n 1} & a_{n 2} & \cdots & a_{n n}
\end{array}\right|
$$
【性质】==6. 把行列式的某一行（列）的各元素乘以同样数然后加到另一行（列）对应的元素上去，行列式不变。==

## 行列式按行（列）展开