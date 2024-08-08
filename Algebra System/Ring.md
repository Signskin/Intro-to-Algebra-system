## 环
### 定义:环
> 设$(R,\oplus,\otimes)$是代数系统,$\oplus,\otimes$是R上两个二元运算,若
> 1. $(R,\oplus)$是交换群
> 2. $(R,\otimes)$是半群
> 3. $\otimes$对$\oplus$有分配律,即
$$
\begin{align}
a\otimes(b\oplus c)=(a\otimes b)\oplus(a\otimes c) \\
(a\otimes b)\oplus(a\otimes c)=a\otimes(b\oplus c)
\end{align}
$$
> 则称$(R,\oplus,\otimes)$是环.

要点:
1. 记群$(R,\oplus)$之幺元为$0$,将每个元素$a$之逆元$a^{-1}$记作$-a$,将$a\oplus b^{-1}$记作$a-b$.即*环上可以定义减法*.
2. 对半群$(R,\otimes)$,若有幺元,则记为$1$或$e$.进而若$a$对$\otimes$可逆,将逆元记为$a^{-1}$.
3. 不讨论单元素环.
4. 不要求$\oplus$对$\otimes$分配.

常见环有$(\mathbb{Z},+,\times),(\mathrm{M}_{n\times n},+,\times),(\mathbb{N}_{n},+_{n},\times_{n}),(2^X,\cap,\cup),(\mathrm{P}[x],+,\times)$,分别是整数环,矩阵环,整数模环,子集环和多项式环.

### 定义:交换环
> 设$(R,\oplus,\otimes)$是环,若$\otimes$有交换律,那么称$(R,\oplus,\otimes)$为交换环.

### 定义:含幺环
> 设$(R,\oplus,\otimes)$是环,若$\otimes$有幺元,那么称$(R,\oplus,\otimes)$为含幺环.

### 定理:环之基本性质
> 1.零元:加法幺元乃乘法零元,即$\forall a,0\otimes a=a\otimes0=0.$
> 2.正负及负正得负:$a\otimes(-b)=(-a)\otimes b=-(a\otimes b).$
> 3.负负得正:$(-a)\otimes(-b)=a\otimes b.$
> 4.乘法对减法运算左右分配.
##### 证明1
$$
0\otimes a=(0\oplus0)\otimes a=(0\otimes a)\oplus(0\otimes a)\implies(0\otimes a)=0.
$$
> 另一侧同理.

##### 证明2
$$
\begin{align}
a\otimes(-b) & =(a\otimes(-b))\oplus0 \\
 & =(a\otimes(-b))\oplus ((a\otimes b) \oplus -(a\otimes b)) \\
 & =(a\otimes(-b\oplus b))\oplus -(a\otimes b) \\
 & =(a\otimes0)\oplus-(a\otimes b) \\
 & =0\oplus-(a\otimes b) \\
 & =-(a\otimes b)
\end{align}
$$
> 另一侧同理.

##### 证明3
$$
(-a)\otimes(-b)=a\otimes(-(-b))=a\otimes b.
$$
> 这是因为$(b^{-1})^{-1}=b$,即群有反身律.
#### 推论:$(R,\otimes)$非群
> 由性质1,乘法有零元.又由[[Group#^fa8570|群无零元]],可知$(R,\otimes)$不成群.


### 定义:含零因子环 不含零因子环
> 设$(R,\oplus,\otimes)$是环,称$(R,\oplus,\otimes)$为含零因子环,若且唯若其满足:
> $\exists a,b\in R,a\neq 0\land b\neq0\land a\otimes b=0$.
> 称$a$为左零因子,$b$为右零因子. 
> 特别地,若$R$是交换环,则$a=b$合称为零因子.

> 设$(R,\oplus,\otimes)$是环,$(R,\oplus,\otimes)$不含零因子(no nil-factor),即为不含零因子环,若且唯若其满足:
> $\forall a,b\in R,a\neq0\land b\neq 0\land a\otimes b\neq 0$.

考虑整数模环$(\mathbb{N}_{m},+_{m},\times_{m})$:
	若$m$是质数,设$\exists[i]_{m}\neq[j]_{m}\neq[0]_{m},[i]_{m}\otimes[j]_{m}=[0]_{m}\implies m|i\times j \implies m|i或m|j$,这与$i,j\neq 0$矛盾.故为无零因子环.
	若$m$是合数,容易知道为有零因子环.
#### 定理:无零因子等价消去
> 设$(R,\oplus,\otimes)$是环,$\otimes$有消去律唯且唯若环无零因子.
### 定义:整环
> 交换含幺无零因子环称为整环,又称整区.

### 定义:除环
> 每个非零元均有乘法逆元之含幺环称为除环.
#### 定理:除环定理(除环必要条件)

^5fe77c

> 除环是含幺无零因子环.

##### 证明:
> 只要证明除环无零因子.
> 反证,设$\exists a,b\in R,a,b\neq 0,a\otimes b=0=0\otimes b\implies$
> $a\otimes b\otimes b^{-1}=0\otimes b\otimes b^{-1}\implies$
> 而$(b\otimes b^{-1})$也有逆元,因其不为零.
> 进而$a=0$,矛盾.
> 故定理成立.

除环和整环无必然关系.

#### 定理:有限除环定理(有限除环充要条件)
> 有限含幺环中,无零因子若且唯若非零元有逆元.
##### 证明:
> 无零因子$\implies$非零元有逆元:
> 	$\otimes$在$R\setminus \{0\}$封闭,故$(R\setminus \{ 0 \},\otimes)$是半群.
> 	由鸽巢原理,$\forall r\in R\setminus \{ 0 \},\exists j>i\in \mathbb{N},$
$$
\begin{align}
r^i=r^j & \implies r^j=r^i \\
 & \implies r^{j-i}\otimes r^i=e\otimes r^i \quad(消去律)\\
 & \implies r^{j-i}=e\quad(无零因子等价消去) \\
 & \implies r^{-1}=r^{j-i-1}
\end{align}
$$
>	即非零元有逆元.
> 非零元有逆元$\implies$无零因子:在[[#^5fe77c|除环定理]]已经证明.
#### 定理:有限整环为除环
> 有限整环为除环.

^deb034

#### 定理:有限除环定理(三等价)
> 对有限含幺环,除环等价于乘法满足消去等价于无零因子.