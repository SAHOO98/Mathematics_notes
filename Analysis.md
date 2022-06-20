[[Latex header]]
# Gamma and Beta function

$$\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt$$
$$\beta(x,y) = \int_0 ^1 t^{x-1}(1-t)^{y-1}dt = 2\int_0 ^{\frac{\pi}{2}} \sin^{2x-1}{\theta} \cos^{2y-1}{\theta} d\theta$$


| Column 1                                                             | Column 2                                             |
| -------------------------------------------------------------------- | ---------------------------------------------------- |
| $\Gamma(z) = (z-1)\Gamma(z-1)$                                       | $\beta(x,y)= \frac{\Gamma(x)\Gamma(y)}{\Gamma(x+y)}$ |
| $\Gamma(n) = (n-1)!$   $,\forall n\in \mathbb{N}$                    | Blank                 |
| $\Gamma(\frac{1}{2}) = \sqrt{\pi}$                                   | Blank                       |
| $\Gamma(n)\Gamma(n+\frac{1}{2}) = 2^{1-2n}\sqrt{\pi}\cdot\Gamma(2n)$ | Blank                 |
| $\Gamma(1-n)\Gamma(n)= \frac{\pi}{\sin{\pi n}}$                      |     Blank

# Sequences
## Defnitions
1. A sequence of real number is a function, $f:\N \rightarrow \R$. Commonly represented as $\sequence{a} = \braces{a_1, a_2, a_3, \cdots}$.

2. A series is a summation of the sequnce elements. Series of above sequence is written as:- $$
A = \sum_{n \in \N} a_n=\sum_{n=1}^{\infty} a_n = a_1+a_2+a_3+\cdots
$$

3. Partial sum of a series can be written as : $$A_n = \sum_{k=1}^{n}a_k$$ Note this is a finite sum of the orginal series $A$.

## Convergence of sequence

Given, $\sequence{a}$ in $\R$. $a\in \R$.
The sequence $\sequence{a}$ converges to $a$ if only if $$\forall \e>0 \exists N \in \N \text{ s.t } n>N \implies|x_n-x|<\e$$.

Syntaxtically, $$\lim a_n = \lim_{n\rightarrow \infty}a_n = a$$

### Properties
Say, $\sequence{s}\ra s$ and $\sequence{t}\ra t$. 
* $\lim s_n + t_n = s+t$
* $\lim c\cdot s_n = c\cdot s$ for all $c \in R$
* $\lim c+ s_n = c+ s$ for all $c \in R$
* $\lim t_n s_n = ts$
* $\lim \frac{1}{s_n} = \frac{1}{s}$ [considering all is well-defined]

### Sepcial sequence 
* if $p>0$ then $\lim \frac{1}{n^p} = 0$
* if $p>0$ then $\lim p^{\frac{1}{n}} = 1$
* $\lim n^{\frac{1}{n}} = 1$
* if $p>0$ and $a \in \R$ then $\lim \frac{n^a}{(1+p)^n} = 0$
* if $|x|<1$ then $\lim x^n = 0$
* $\lim (1+n)^{1/n} = 1$

## Convergence of Series
Let, 
$$A = \sum_n a_n$$ $$ A_n= \sum_{k=1}^{n} a_k$$
See carefully that, series $A$ 's convergence is same as convergence of the following sequence of partial sums: $\braces{A_1, A_2, A_3...}$. So more formally one can write, $$\lim_{n \ra \infty} A_n = A$$

So all the techniques used in convergence of sequence can be used here too.

## Properties
$$\R$$