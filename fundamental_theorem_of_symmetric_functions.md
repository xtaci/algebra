证明：任意的对称多项式都可以表达为基本对称多项式的多项式。

对变量的个数 $n$ 进行归纳：

当 $n = 1$ 时，结论成立；

假设 $n-1$ 个变量时结论成立，下面证明 $n$ 个变量时结论也成立。

用 $\sigma_k=\sum_{1\leq i_1\leq i_2\leq\cdots\leq i_k\leq n}x_{i_1}x_{i_2}\cdots x_{i_k}$ , $1\leq k\leq$ $n$ 来表示 $n$ 元基本对称多项式。

用 $\tau_k=\sum_{1\leq i_1\leq i_2\leq \dots\leq i_k\leq n-1}x_{i_1}x_{i_2}\cdots x_{i_k}$, $1\leq k\leq$ $n-1$ 来表示 $n-1$ 元基本对称多项式。

$\sigma_1=\tau_1+x_n\Rightarrow \tau_1=\sigma_1-x_n$

$\sigma_2=\tau_2+\tau_1 x_n\Rightarrow \tau_2=\sigma_2-x_n\sigma_1+x_n^2$

$\sigma_3=\tau_3+\tau_2 x_n\Rightarrow \tau_3=\sigma_3-\sigma_2 x_n+\sigma_1x_n^2-x_n^3$

...

$\sigma_{n-1}=\tau_{n-1}+\tau_{n-2}x_n\Rightarrow \tau_{n-1}=\sigma_{n-1}-\sigma_{n-2}x_n+\cdots+(-1)^k\sigma_{n-k-1}x_n^k+\cdots+(-1)^nx_n^{n-1}$

$\sigma_n=\tau_{n-1}x_n\Rightarrow 0=\sigma_n-\sigma_{n-1}x_n+\cdots+(-1)^n\sigma_1x_n^{n-1}+(-1)^{n+1}x_n^n$

可以发现，任意 $n$ 次的多项式，都可以整理为以 $x_n^k, k \leq n-1$ 次的基本多项式作为系数的多项式，写为：

$f=g_{n-1}x_n^{n-1}+\cdots+g_1x_n+g_0$ ( $0\leq k\leq n-1$ ) . 
其中 $g_k\in F(x_1,x_2,\cdots, x_{n-1}),0\leq k\leq n-1$

由于 $f$ 是 $n$ 元对称多项式, 意味着 $n$ 个元素任意对换是对称的，那么保持其中的一个元素 $x_n$ 不动，只兑换其他 $k < n$ 的 $x_k$ 元素，当然也依然对称（部分小于整体）， 可得 $f$ 在 $x_1,x_2,\cdots, x_{n-1}$ 的任意置换下不变，由此可得所有系数 $g_k$ 均不改变，均为 $n-1$ 元对称多项式。

