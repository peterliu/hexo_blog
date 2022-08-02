---
title: Markdown数学公式语法整理
tags:
cover: /cover-image/math-1509228468518-180dd4864904.jpg
---

本文介绍在 Markdown 文件中书写数学公式的方法

<!-- more -->

![](/cover-image/math-1509228468518-180dd4864904.jpg)


### 行内与独行
类型    |    示例 、作用    |    符号    |    写法
----    |    ----    |    ----   |    ----
行内公式 | 将公式插入到本行内   |  `$ ... $`  | `$ 公式 $`
独行公式 | 将公式插入到新的一行内，并且居中 | `$$ ... $$` | `$$ 公式 $$`


### 上标、下标与组合
类型    |    示例    |    符号    |    写法
----    |    ----    |    ----   |    ----
上标符号 |   $x^2$    |    ^     |    x^2
下标符号 |   $x_1$    |    _     |    x_1
组合符号 |  $x^{a+b}$  |  {...}  |   x^{a+b}  


### 汉字、字体与格式
类型    |    示例    |    符号    |    写法
----    |    ----    |    ----   |    ----
汉字形式 | $V_{\mbox{初始}}$ | \mbox{} | V_{\mbox{初始}}
字体控制 | $\displaystyle \frac{x+y}{y+z}$ | \displaystyle | \displaystyle \frac{x+y}{y+z}
下划线  | $\underline{x+y}$ | \underline | \underline{x+y}
标签    | $\tag{1}$ | \tag{} | \tag{1}
上大括号 | $\overbrace{a+b+c+d}^{2.0}$ | \overbrace{算式} | \overbrace{a+b+c+d}^{2.0}
下大括号 | $a+\underbrace{b+c}_{1.0}+d$ | \underbrace{算式} | a+\underbrace{b+c}_{1.0}+d
上位符号 | $\vec{x}\stackrel{\mathrm{def}}{=}{x_1,\dots,x_n}$ | \stacrel{上位符号}{基位符号} | \vec{x}\stackrel{\mathrm{def}}{=}{x_1,\dots,x_n}


### 占位符
类型    |    示例    |    符号    |    写法
----    |    ----    |    ----   |    ----
紧贴    |  $x \! y$   |    \!     |    x \! y
没有空格|    $xy$     |           |    xy
小空格  |  $x , y$   |    ,      |     x , y
中空格  |  $x : y$   |    :      |     x : y
大空格  |  $x \ y$   |    \      |     x \ y
quad空格|  $x \quad y$  | \quad  |  x \quad y
两个quad空格|  $x \qquad y$  | \qquad  |  x \qquad y


### 定界符与组合
类型    |    示例    |    符号    |    写法
----    |    ----    |    ----   |    ----
括号    |    $()$    |     ()    |    () 
不同大小的括号 | $\big( \Big( \bigg( \Bigg($ | \big \Big \bigg \Bigg | \big( \Big( \bigg( \Bigg(
中括号  |  $[x+y]$   |    []     |    [x+y]
大括号  |  ${x+y}$   |    { }    |    {x+y}
自适应括号| $\left(x{yz}\right)$ | \left \right | \left(x{yz}\right)
组合公式| ${n+1 \choose k}={n \choose k}+{n \choose k-1}$ | | {n+1 \choose k}={n \choose k}+{n \choose k-1}
组合公式| $\sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots$ | | \sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots


### 四则运算
类型    |    示例    |    符号    |    写法
----    |    ----    |    ----   |    ----
加法运算 |  $z=x+y$  |     +      |    z=x+y
减法运算 |  $z=x-y$  |     +      |    z=x-y
加减运算 |  $z=x \pm y$  |     \pm      |    z=x \pm y
减加运算 |  $z=x \mp y$  |     \mp      |    z=x \mp y
乘法运算 |  $z=x \times y$  |     \times      |    z=x \times y
点乘运算 |  $z=x \cdot y$  |     \cdot      |    z=x \cdot y
星乘运算 |  $z=x * y$  |     *     |    z=x * y
星乘运算 |  $z=x \ast y$  |    \ast     |    z=x \ast y
除法运算 |  $z=x / y$  |     /     |    z=x / y
除法运算 |  $z=x \div y$  |     \div     |    z=x \div y
分式表示 | $\frac{x+y}{y+z}$ | \frac | \frac{x+y}{y+z}
分式表示 | ${x+y} \over {y+z}$ | {分子} \voer {分母} | {x+y} \over {y+z}
绝对值   | $\|x+y\|$   |   \|\|    |    \|x+y\|


### 高级运算
类型    |    示例    |    符号    |    写法
----    |    ----    |    ----   |    ----
平均数  |  $\overline{xyz}$  | \overline |  \overline{xyz}
开平方  |  $\sqrt{2}$  |  \sqrt{}  |  \sqrt{2}
开方    |  $\sqrt[n]{x}$  |  \sqrt[开方数]{被开方数}  |  \sqrt[n]{x}
对数    |  $\log{x}$  |  \log{}  |    \log{x}
对数    |  $\log _n{x}$  |  \log _底数 {数}  |    \log _n{x}
极限    |  $\lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$ | \lim ^{上标} _{下标} {表达式} | \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}
极限    |  $\displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$ | | \displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}
求和    |  $\sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}$  |  \sum  |  \sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}
求和    |  $\displaystyle \sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}$  |  \sum  |  \displaystyle \sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}
积分    |  $\int^{\infty}_{0}{xdx}$  |  \int   |   \int^{\infty}_{0}{xdx}
积分    |  $\displaystyle \int^{\infty}_{0}{xdx}$  |  \int  |  \displaystyle \int^{\infty}_{0}{xdx}
微分    |  $\frac{\partial x}{\partial y}$   |  \partial  |  \frac{\partial x}{\partial y}



矩阵    
$$\left[ \begin{matrix} 1 &2 &\cdots &4\5 &6 &\cdots &8\\vdots &\vdots &\ddots &\vdots\13 &14 &\cdots &16\end{matrix} \right]$$




### 逻辑运算
类型       |    示例    |    符号    |    写法
----      |    ----    |    ----   |    ----
等于       |  $z=x+y$   |    =     |    z=x+y
不等于    |  $z \neq x+y$   |    \neq      |    z \neq x+y
大于      |  $z>x+y$   |    >     |    z>x+y
小于      |  $z<x+y$   |    <     |    z<x+y
大于等于  |  $z \geq x+y$   |    \geq     |    z \geq x+y
小于等于  |  $z \leq x+y$   |    \leq     |    z \leq x+y
不大于等于|  $z \ngeq x+y$   |    \ngeq      |    z \ngeq x+y
不大于等于|  $z \not \geq x+y$   |    \not \geq      |    z \not \geq x+y
不小于等于|  $z \nleq x+y$   |    \nleq      |    z \nleq x+y
不小于等于|  $z \not \leq x+y$   |    \not \leq      |    z \not \leq x+y
约等于    |  $z \approx x+y$   |    \approx     |    z \approx x+y
恒等于    |  $z \equiv x+y$   |    \equiv     |    z \equiv x+y



### 集合运算
类型       |    示例    |    符号    |    写法
----      |    ----    |    ----   |    ----
属于       |   $x \in y$   |   \in    |  x \in y
不属于     |   $x \notin y$   |   \notin    |  x \notin y
不属于     |   $x \not \in y$   |   \not \in    |  x \not \in y
子集       |   $x \subset y$   |  \subset  | x \subset y
子集       |   $x \supset y$   |  \supset  | x \supset y
真子集     |   $x \subseteq y$  | \subseteq | x \subseteq y
非真子集   |   $x \subsetneq y$  | \subsetneq | x \subsetneq y
真子集     |   $x \supseteq y$  | \supseteq | x \supseteq y
非真子集   |   $x \supsetneq y$  | \supsetneq | x \supsetneq y
非子集     |   $x \not \subset y$ | \not \subset | x \not \subset y
非子集     |   $x \not \supset y$ | \not \supset | x \not \supset y
并集       |   $x \cup y$    | \cup | x \cup y
交集      |   $x \cap y$    | \cap | x \cap y
差集      |   $x \setminus y$    | \setminus | x \setminus y
同或      |   $x \bigodot y$    | \bigodot | x \bigodot y
同与      |   $x \bigotimes y$    | \bigotimes | x \bigotimes y
实数集合   |  $\mathbb{R}$  | \mathbb{R} |  \mathbb{R}
自然数集合 |  $\mathbb{Z}$  | \mathbb{Z} |  \mathbb{Z}
空集      |  $\emptyset$  | \emptyset |  \emptyset


### 数学符号
类型       |    示例    |    符号    |    写法
----      |    ----    |    ----   |    ----
无穷       |  $\infty$  |  \infty  | \infty
虚数       |  $\imath$  |  \imath  | \imath
虚数       |  $\jmath$  |  \jmath  | \jmath
数学符号   |  $\hat{a}$  |  \hat  | \hat{a}
数学符号   |  $\check{a}$  |  \check  | \check{a}
数学符号   |  $\breve{a}$  |  \breve  | \breve{a}
数学符号   |  $\tilde{a}$  |  \tilde  | \tilde{a}
数学符号   |  $\bar{a}$  |  \bar  | \bar{a}
矢量符号   |  $\vec{a}$  |  \vec  | \vec{a}
数学符号   |  $\acute{a}$  |  \acute  | \acute{a}
数学符号   |  $\grave{a}$  |  \grave  | \grave{a}
数学符号   |  $\mathring{a}$  |  \mathring  | \mathring{a}
一阶导数符号   |  $\dot{a}$  |  \dot  | \dot{a}
二阶导数符号   |  $\ddot{a}$  |  \ddot  | \ddot{a}
上箭头    |  $\uparrow$  |  \uparrow  | \uparrow
上箭头    |  $\Uparrow$  |  \Uparrow  | \Uparrow
下箭头    |  $\downarrow$  |  \downarrow  | \downarrow
下箭头    |  $\Downarrow$  |  \Downarrow  | \Downarrow
左箭头    |  $\leftarrow$  |  \leftarrow  | \leftarrow
左箭头    |  $\Leftarrow$  |  \Leftarrow  | \Leftarrow
右箭头    |  $\rightarrow$  |  \rightarrow  | \rightarrow
右箭头    |  $\Rightarrow$  |  \Rightarrow  | \Rightarrow
底端对齐的省略号    |  $1,2,\ldots,n$  |  \ldots  | \ldots
中线对齐的省略号    |  $x_1^2 + x_2^2 + \cdots + x_n^2$  |  \cdots  | \cdots
竖直对齐的省略号    |  $\vdots$  |  \vdots  | \vdots
斜对齐的省略号      |  $\ddots$  |  \ddots  | \ddots


### 希腊字母
字母  |  实现  |  字母  |  实现
---   |  ---  |  ---  | ---
A  |  A  |  α  |  \alhpa
B  |  B  |  β  |  \beta
Γ  |  \Gamma  |  γ  |  \gamma
Δ  |  \Delta  |  δ  |  \delta
E  |  E  |  ϵ  |  \epsilon
Z  |  Z  |  ζ  |  \zeta
H  |  H  |  η  |  \eta
Θ  |  \Theta  |  θ  |  \theta
I  |  I  |  ι  |  \iota
K  |  K  |  κ  |  \kappa
Λ  |  \Lambda  |  λ  |  \lambda
M  |  M  |  μ  |  \mu
N  |  N  |  ν  |  \nu
Ξ  |  \Xi  |  ξ  |  \xi
O  |  O  |  ο  |  \omicron
Π  |  \Pi  |  π  |  \pi
P  |  P  |  ρ  |  \rho
Σ  |  \Sigma  |  σ  |  \sigma
T  |  T  |  τ  |  \tau
Υ  |  \Upsilon  |  υ  |  \upsilon
Φ  |  \Phi  |  ϕ  |  \phi
X  |  X  |  χ  |  \chi
Ψ  |  \Psi  |  ψ  |  \psi
Ω  |  \v  |  ω  |  \omega


### 方程式组

```
$$ 
\left\{
    \begin{aligned} 
        x + y + z &= 3    \\
        {\partial{x} \over y^\prime} &= {{x+1} \over {y-1}}        \\
        \frac{y}{z} &= 2
    \end{aligned}
\right.
$$


$$ 
\begin{cases} 
    x + y + z &= 3    \\
    {\partial{x} \over y^\prime} &= {{x+1} \over {y-1}}        \\
    \frac{y}{z} &= 2
\end{cases} 
$$
```

$$ x + y + z = 3 $$

