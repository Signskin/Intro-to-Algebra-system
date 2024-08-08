## 域
### 定义:域
> 设$(F,\oplus,\otimes)$是代数系统,$\otimes,\oplus$是$F$上两个二元运算,称$F$是域,若且唯若
> 1. $(F,\oplus)$是交换群
> 2. $(F\setminus \{ 0 \},\otimes)$是交换群
> 3. $\otimes$对$\oplus$满足(单侧)分配律

常见域有有理数域$\mathbb{Q}$,实数域$\mathbb{R}$,复数域$\mathbb{C}$,算术分类域$S_{P_{k}}(\{ a+b \sqrt{ P_{k} },a,b\in \mathbb{Q} \},+,\times)$,其中$P_{k}$是第$k$个素数.
在环的基础上,对乘法还要求:可交换,有幺元及除0可逆.
##### 补充:证明算术分类域$S_{2}$乘法是封闭的
$$
\forall a,b,c,d\in \mathbb{Q},
$$
#### 定理:可交换除环是域(充要条件,可作定义)
> 可交换除环是域.

##### 证明:
> 由除环定义,其实$(F,\otimes)$已经成含幺且除0可逆群,则只要可交换就是域.
#### 定理:有限整环是域
> 有限整环是域.

在有限条件下,域等价于有限整环.而在无限条件下,***域是整环,整环未必是域***.
##### 证明:
由[[Ring#^deb034|有限整环为除环]],及整环满足交换,则有限整环为域.