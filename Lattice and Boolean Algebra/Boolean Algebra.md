## 布尔代数
### 定义:布尔代数
> 有补的分配格$(B,\preceq,\land,\lor,',0,1)$称为*布尔代数*.

##### 例
> 集合代数$(2^X,\subseteq,\cap,\cup,',\varnothing,X)$是布尔代数.

> 电路通断$\{ 0,1 \}$,同运算与$\land$或$\lor$非$!$共同构成的格是布尔代数,称为开关代数.

> 命题真假$\{ F,T \}$,同运算合取,析取,否定构成的格是布尔代数,称为命题代数.

#### 定理:三种代数同构
> *n元集合代数*同构于*n元开关代数*同构于*n元命题代数*.

#### 定理:布尔代数的性质
> 设$(B,\preceq,\land,\lor,',0,1)$是布尔代数.
> 1.反身律$\forall a\in B,(a')'=a$.
> 2.消去律:$\forall a,b,c$
$$
a\land b=a\land c且a'\land b=a'\land c\implies b=c
a\lor b=a\lor且a'\lor b=a'\lor c\implies b=c
$$
> 3.De Morgan律:$(a\land b)'=a'\lor b'$;$(a\lor b)'=a'\land b'$.

#### 定理:布尔代数的运算
> 设有布尔代数$(B,\preceq,\land,\lor,',0,1)$,则以下四命题等价:
> 1. $a\preceq b$
> 2. $b'\preceq a'$
> 3. $a\land b'=0$
> 4. $a'\lor b=1$







