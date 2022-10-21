
# 第一章 函数与极限

## 1.1 映射与函数（Mappings and functions）

### 1.1.1 映射

==*集合*==

**集合**：具有某种特定性质的事物。

**元素**：组成集合的事物。

**空集**：不含任何元素的集合，记作 $\varnothing$ 。

- 元素 $a$ 属于集合 $M$ ，记作 $a \in M$
- 元素 $a$ 不属于集合 $M$ ，记作 $a \notin M$

集合表示方法：

1. 列举法
2. 描述法

> 两个整数**互质（互素）**：没有大于 $1$ 的整数公因子。

==*集合之间的关系*==

**子集**：设有集合 $A$ 和 $B$ ，若 $x \in A$ 必有 $x \in B$ ，则 $A$ 是 $B$ 的子集（ $B$ 包含 $A$ ），记作 $A \subset B$ 。

**相等**：若 $A \subset B$ 且 $B \subset A$ ，则  $A$ 与 $B$ 相等，记作 $A=B$。

==*集合之间的运算*==

**并集**：$A \cup B=\{x \mid x \in A$ 或 $x \in B\}$

**交集**：$A \cap B=\{x \mid x \in A$ 且 $x \in B\}$

**差集**：$A \backslash B=\{x \mid x \in A$ 且 $x \notin B\}$

<div align=center>
  <img src="images\1_1_1_1.png" height="50%" width="50%">
</div>

==*区间*==

**区间**：介于某两个实数（区间的端点）之间的全体实数。

$\forall a, b \in R$, 且 $a<b$

- 有限区间：
  - 开区间： $\{x \mid a<x<b\}$ ，记作 $(a, b)$

    <div align=center>
      <img src="images\1_1_1_2.png" height="50%" width="50%">
    </div>

  - 闭区间： $\{x \mid a \leq x \leq b\}$ ，记作 $[a, b]$

    <div align=center>
      <img src="images\1_1_1_3.png" height="50%" width="50%">
    </div>

  - 半开区间：

    -  $\{x \mid a \leq x<b\}$ ，记作 $[a, b)$
    -  $\{x \mid a<x \leq b\}$ ，记作 $(a, b]$

- 无限区间：
  -  $[a,+\infty)=\{x \mid a \leq x\}$
  - $(-\infty, b)=\{x \mid x<b\}$

==*邻域*==

**点 $x_0$ 的 $\delta$ 邻域**：

设 $x_0 \in \mathrm{R}$ 

$U\left(x_0, \delta\right)=\left\{x|| x-x_0 \mid<\delta\right\}$
$=\left\{x \mid x_0-\delta<x<x_0+\delta\right\}$
$=\left(x_0-\delta, x_0+\delta\right)$

**点 $x_0$ 的 $\delta$ 去心邻域**：

$\stackrel{\circ}{U}\left(x_0, \delta\right)=\left\{x|0<| x-x_0 \mid<\delta\right\}$
$\quad=\left\{x \mid x_0-\delta<x<x_0+\delta, x \neq x_0\right\}$
$\quad=\left(x_0-\delta, x_0\right) \cup\left(x_0, x_0+\delta\right)$

==*逻辑量词*==

全称量词：任意，记作 $\forall$

存在量词：存在，记作 $\exists$

**映射**：设 $X$ ， $Y$ 是集合。若 $\forall x \in X$ ， $\exists$ 唯一的 $y \in Y$ ，使得 $f: x \rightarrow y$ ，则称 $f$ 为 $X$ 到 $Y$ 的一个映射。记作：
$$
f: X \rightarrow Y
$$

- **对应法则**： $f$
- **定义域**： $D_f=X$
- **值域**： $R_f=f(X)=\{f(x)|x \in X\}$

**满射**： $f: X \rightarrow Y$ ， $\forall y \in Y, \quad \exists x \in X \Longrightarrow f(x)=y$

<div align=center>
  <img src="images\1_1_1_4.png" height="50%" width="50%">
</div>

> $Y$ 中每一个元素都是映射 $f$ 的像

**非满射**： $f: X \rightarrow Y$ ， $\exist y \in Y, \quad \forall x \in X \Longrightarrow y \neq f(x)$

<div align=center>
  <img src="images\1_1_1_5.png" height="50%" width="50%">
</div>

> $Y$ 中存在一个元素不是映射 $f$ 的像

**单射**： $f: X \rightarrow Y$ ， $\forall a, b \in X,a \neq b \Longrightarrow f(a) \neq f(b)$

<div align=center>
  <img src="images\1_1_1_6.png" height="50%" width="50%">
</div>

> 不同的元素有不同的像

**非单射**： $f: X \rightarrow Y$ ， $\exist a, b \in X,a \neq b \Longrightarrow f(a) = f(b)$

<div align=center>
  <img src="images\1_1_1_7.png" height="50%" width="50%">
</div>

> 至少存在两个不同的元素有相同的像

**双射**： $f: X \rightarrow Y$ ，即是单射又是满射（一一映射）。

<div align=center>
  <img src="images\1_1_1_8.png" height="50%" width="50%">
</div>

- $\color{red}{每一个单射可以诱导一个双射}$

若 $f: X \rightarrow Y$ 是单射，则 $f: X \rightarrow f(X)$ 是双射。

<div align=center>
  <img src="images\1_1_1_9.png" height="50%" width="50%">
</div>

- $\color{red}{每一个单射可以诱导逆映射}$

若 $f: X \rightarrow Y$ 是单射，则 $f: X \rightarrow Y$ 可逆。

**逆映射**：若 $\forall y \in f(X)$ ， $\exists$ 唯一的 $x \in X$ ，使得 $f^{-1}: y \rightarrow x$ 。记作：
$$
f^{-1}: f(X) \rightarrow X
$$

<div align=center>
  <img src="images\1_1_1_10.png" height="50%" width="50%">
</div>

### 1.1.2 函数

**函数**：数集 $X$ 到数集 $R$ 的映射：
$$
f: X \rightarrow R
$$
其中 $X \subseteq R$

------

设 $f: x \rightarrow y$ ，记作 $y=f(x)$ 

对于 $f: X \rightarrow Y$

- **对应法则**： $f$
- **定义域**： $D_f=X$
- **值域**： $R_f=f(X)=\{f(x)|x \in X\}$

**反函数**：若函数 $y=f(x)$ 是单映射（ $x_1 \neq x_2 \Rightarrow f\left(x_1\right) \neq f\left(x_2\right)$ ），则函数 $f$ 可逆，且（逆映射）反函数为 $x=f^{-1}(y)$ （仍是单映射） 。

==*几个重要的分段函数*==

绝对值函数：
$$
y=|x|= \begin{cases}x & x \geq 0 \\ -x & x<0\end{cases}
$$

<div align=center>
  <img src="images\1_1_2_1.png" height="50%" width="50%">
</div>

符号函数：
$$
y=\operatorname{sgn} x= \begin{cases}-1, & x<0, \\ 0, & x=0, \\ 1, & x>0\end{cases}
$$

<div align=center>
  <img src="images\1_1_2_2.png" height="50%" width="50%">
</div>

取整函数：
$$
y=[x]
$$

<div align=center>
  <img src="images\1_1_2_3.png" height="50%" width="50%">
</div>

$\forall x \in R$ ， $[x] \leq x<[x]+1$

$\forall x \in R$ ， $x=[x]$当且仅当 $x$ 是整数

## 1.2 数列的极限

### 1.2.1 数列极限的定义

### 1.2.2 收敛数列的性质

## 1.3 函数的极限

### 1.3.1 函数极限的定义

### 1.3.2 函数极限的性质

## 1.4 无穷小和无穷大

### 1.4.1 无穷小

### 1.4.2 无穷大

## 1.5 极限运算法则

## 1.6 极限存在准则 两个重要极限

## 1.7 无穷小的比较

## 1.8 函数的连续性与间断点

### 1.8.1 函数的连续性

### 1.8.2 函数的间断点

## 1.9 连续函数的运算与初等函数的连续性

### 1.9.1 连续函数的和、差、积、商的连续性

### 1.9.2 反函数与复合函数的连续性

### 1.9.3 初等函数的连续性

## 1.10 闭区间上连续函数的性质

### 1.10.1 有界性与最大值最小值定理

### 1.10.2 零点定理与介值定理

### 1.10.3 一致连续性