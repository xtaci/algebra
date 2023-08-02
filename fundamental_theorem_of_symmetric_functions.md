证明：任意的对称多项式都可以表达为基本对称多项式的多项式。

用 $\sigma_k=\sum_{1\leq i_1\leq i_2\leq\cdots\leq i_k\leq n}x_{i_1}x_{i_2}\cdots x_{i_k}$ , $1\leq k\leq$ $n$ 来表示 $n$ 元基本对称多项式。

用 $\tau_k=\sum_{1\leq i_1\leq i_2\leq \dots\leq i_k\leq n-1}x_{i_1}x_{i_2}\cdots x_{i_k}$, $1\leq k\leq$ $n-1$ 来表示 $n-1$ 元基本对称多项式。

$\sigma_1=\tau_1+x_n\Rightarrow \tau_1=\sigma_1-x_n$

$\sigma_2=\tau_2+\tau_1 x_n\Rightarrow \tau_2=\sigma_2-x_n\sigma_1+x_n^2$

$\sigma_3=\tau_3+\tau_2 x_n\Rightarrow \tau_3=\sigma_3-\sigma_2 x_n+\sigma_1x_n^2-x_n^3$

...

$\sigma_{n-1}=\tau_{n-1}+\tau_{n-2}x_n\Rightarrow \tau_{n-1}=\sigma_{n-1}-\sigma_{n-2}x_n+\cdots+(-1)^k\sigma_{n-k-1}x_n^k+\cdots+(-1)^nx_n^{n-1}$

$\sigma_n=\tau_{n-1}x_n\Rightarrow 0=\sigma_n-\sigma_{n-1}x_n+\cdots+(-1)^n\sigma_1x_n^{n-1}+(-1)^{n+1}x_n^n$

注意最后这里的：

$0=\sigma_n-\sigma_{n-1}x_n+\cdots+(-1)^n\sigma_1x_n^{n-1}+(-1)^{n+1}x_n^n$

调整一下等式，可以得到：

$-(-1)^{n+1}x_n^n=\sigma_n-\sigma_{n-1}x_n+\cdots+(-1)^n\sigma_1x_n^{n-1}$

即: 基本对称多项式中的 $x_n^n$ 可以由最高次项为 $x_n^{n-1}$ 的多项式表达出来，且这个多项式系数是 $\sigma_k$，即基本对称多项式。（推论1）

对于任意一个N元对称多项式，可以转换为一个关于 $x_n$ 的多项式, 他的最高次最大为N次。如: $f(x_n) = \alpha_n \cdot x_n^n + \alpha_{n-1} \cdot x_n^{n-1} + \cdots +  \alpha_1 \cdot x_n + \alpha_0$

那么，根据上面推论1，每一项 $\alpha_{k} \cdot x_n^k$ 都可以变换为一个最高次为 $x_n^{k-1}$ 的对称多项式表达出来：

$f=g_{n-1}x_n^{n-1}+\cdots+g_1x_n+g_0$

由于 $f$ 是 $n$ 元对称多项式, 意味着$n$个元素任意对换是对称的，那么保持其中的一个元素 $x_n$ 不动，只兑换其他元素，也依然对称， 可得 $f$ 在 $x_1,x_2,\cdots, x_{n-1}$ 的任意置换下不变，由此可得 $g_k$ 是 $n-1$ 元对称多项式。

