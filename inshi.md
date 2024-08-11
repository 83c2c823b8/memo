- Lebesgueの収束定理
$$|f_n| \le F ,FはX上可積分\Longrightarrow \lim_{n\to\infty}\int_X f_n(x) d\mu(x) =\int_X\lim_{n\to\infty} f_n(x) d\mu(x) $$
$\displaystyle f:可積分とは\int_{X}|f(x)| d\mu(x) < \infty$

- WeierstrassのM判定法

$\displaystyle\sum_{n}f_n(x) は,|f_n(x)|\le M_n かつ\sum_n M_n < \infty$なら一様収束する. 

### 直交行列 $\xrightarrow{拡張}$ ユニタリ行列
定義:$$A{}^t\!A ={}^t\!AA = I$$ 

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
定義:$$A ={}^t\!A$$ 

- $\braket{Ax,y} = \braket{x,Ay}$
- 固有値は実数
- 直交行列で対角化可能
つまり,固有空間が直交している.

### 交代行列(歪対称行列)$\xrightarrow{拡張}$歪エルミート行列

### 正規行列
定義:$$AA^* = A^*A$$
