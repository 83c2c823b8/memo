- Lebesgueの収束定理
$$|f_n| \le F ,FはX上可積分\Longrightarrow \lim_{n\to\infty}\int_X f_n(x) d\mu(x) =\int_X\lim_{n\to\infty} f_n(x) d\mu(x) $$
$\displaystyle f:可積分とは\int_{X}|f(x)| d\mu(x) < \infty$

- WeierstrassのM判定法

$\displaystyle\sum_{n}f_n(x) は,|f_n(x)|\le M_n かつ\sum_n M_n < \infty$なら一様収束する. 

### 直交行列 $\xrightarrow{拡張}$ ユニタリ行列
定義:
$$A{}^t\!A ={}^t\!AA = I$$ 

- $\det A = \pm 1$
- $AB$も直交行列
- $A^{-1}$も直交行列
- ${}^t\! A$も直交行列
- 対角化可能
- 各,列ベクトル・行ベクトルはONB
- ||Ax|| = ||x||
- $\braket{Ax,Ay}= \braket{x,y}$
- $|\lambda|=1$

### 対称行列  $\xrightarrow{拡張}$エルミート行列
定義:
$$A ={}^t\!A$$ 

- $\braket{Ax,y} = \braket{x,Ay}$
- 固有値は実数
- 直交行列で対角化可能
つまり,固有空間が直交している.

### 交代行列(歪対称行列)$\xrightarrow{拡張}$歪エルミート行列
定義:$$A =-{}^t\!A$$ 

- 対角化可能で固有値は純虚数(0含む)
- $\braket{Ax,y}=-\braket{x,Ay}$

### 正規行列
定義:
$$AA^* = A^* A$$

- $正規行列\Longleftrightarrow ||Ax|| = ||A^* x||$  
- $正規行列\Longleftrightarrow$ユニタリ行列で対角化可能
- 正規行列の固有値の絶対値が1であればユニタリ行列
- 正規行列の固有値の実数であればエルミート行列
- 正規行列の固有値の純虚数であれば歪エルミート行列

**上3つが正規行列であることは容易にわかる**

- $正規行列\Longleftrightarrow ||Ax|| = ||A^* x||$  

($\Longrightarrow$)
$$||Ax||^2 = \braket{Ax,Ax} = \braket{x,A* Ax} = \braket{x,AA^* x}= \braket{A^* x, A^* x}= ||A^* x||^2$$

($\Longleftarrow$)
$$\braket{x,y}=\frac14(||x+y||^2 - ||x-y||^2 + i||x-iy||^2 - ||x+iy||^2)$$
から$\braket{Ax,Ay}=\braket{A^* x, A^* y}$がわかる.
$$\braket{x,A^* Ay}= \braket{x,AA^* y}$$が任意の$x,y$で成り立つので$AA^* = A^* A$

- $正規行列\Longleftrightarrow$ユニタリ行列で対角化可能

($\Longrightarrow$)
任意の行列はユニタリ三角化可能(帰納法で示される)ので,三角行列かつ正規行列は対角行列なのでok.

($\Longleftarrow$)
$B = U^* AU$と対角化されたとする.
$$AA^* = UBU^* (UBU^*)^* = UBU^* UB^* U^* = UBB^* U^* = UB^* B U^* = UB^*U^* UB U^* = (UBU^* )^* UBU^* = A^* A$$
$UU^* = I$とか$BB^* = B^* B$とか使った.
