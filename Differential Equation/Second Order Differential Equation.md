[[Latex header]]

# Types of DE
## Linear DE with constant coeffcient :-


$$
\begin{align}
a_0 \diff yxn + a_1 \diff yx{n-1}+a_2\diff yx{n-2}+ \cdots + a_{n-1}\diff yx{} +a_n y &= Q\\
\implies \sum_{i=0}^n a_i \diff yx {n-i} &=Q, \braces{a_j} \in \R \\
\implies \sum_{i=0}^n a_{n-i} \diff yx {i} &=Q \\
\implies \sum_{i=0}^n a_{n-i} D^iy &=Q \\
\implies f(D)y &=Q \text { where, } D^i =  \diff{}{x}{i}
\end{align}\tag{1}
$$
If $Q \equiv0$ then  the DE is called **homogenous equation** otherwise **non-homogenous**.
### General Solution/ Complete solution
$$f(D) = Q$$ This equation can be solved by conjugation of Complementary fucntion and particular integral.
### Complementary Function(C.F)
To find complementary fucntion from(1), we need to do $Q\equiv 0$, $y=1$  and $D = m$ in (1) to get a $n^{th}$ degree polynomial as following:
$$\sum_i a_{n-i} m^i = 0\tag{2}$$
Let  $\braces{m_i}_{i=1}^n$ be the roots of (2). The value of C.F will depend on the natue of the roots.
1. When $\braces{m_i}_{i=1}^n$ are all real and distinct:	$$C.F = \sum_i c_i e^{m_ix}$$
2. When some roots repeat: Say $m_1 = m_2=m_3=m$ ,then   $$C.F= (c_1+c_2x+c_3x^2)e^m + \sum_{i=4}^n c_i e^{m_ix}$$More generally, if $k$ roots repeat out of $n$ roots then $$C.F = \left(\sum_{j=1}^k c_jx^{j-1}\right)e^{mx} + \sum_{i=k+1}^n c_i e^{m_ix}$$
3. When roots contains complex conjugates. Say out of $n$ roots $k$ are complex roots then $$C.F = \summ{i=1}{k/2}e^{\alpha_ix}\left(c_i\cos(\beta_ix)+ k_i\cos(\beta_ix) \right) + \summ{i=k+1}{n}c'_ie^{m_ix}$$ **Note:-** The complex roots comes in pairts as $m_j = \alpha_j \pm \beta_j$ . Hence the first summation is from 1 to k/2.

### Particular Integral(P.I)
$$P.I = \frac 1{f(D)} .Q$$ From equation (1). Following are the rules for evaluating P.I:
1. $f(D) =D$ $$P.I = \frac 1D Q = \int Q\cdot dx$$
2. (Most general process) $f(D) = D-a$ $$P.I = e^{ax}\int e^{-ax}Qdx$$
Suppose $$P.I = \frac 1 {(D-a)(D-b)}Q = \frac 1{D-a}\left[e^{bx} \int e^{-bx}dx \right]=e^{ax}\int e^{-ax}\left[e^{bx} \int e^{-bx}dx\right]dx$$

3. If $Q = e^{ax}$ , where $a \in \R$ . If $f(a)\neq 0$, then $$P.I  = \frac 1{f(D)}e^{ax} = \frac{e^{ax}}{f(a)}$$Now, if $f(a) = 0 \implies f(D) = (D-a)^n \phi(D)$ such that $\phi(a)\neq 0$ for some $n \in \N$. $$\begin{align} P.I &= \frac 1{(D-a)^n \phi(D)} e^{ax} \\
 &= \frac 1 {\phi(D)} \left[\frac {e^{ax}}{(D-a)^n}\right]\\
 &= \frac 1 {\phi(D)} \left[\frac {x^ne^{ax}}{n!}\right] \text{ [Using the Rule.2 from above]} \\ 
 &= \frac 1 {\phi(a)} \left[\frac {x^ne^{ax}}{n!}\right] \end{align}$$

4. If $Q = \sin(ax)$ or   $Q = \cos(ax)$. Substitute $D^2 \ra -a^2$. Similarly $D^3 \ra -a^2D$ $$P.I = \frac 1 {f(D)} Q$$**Note:- after the substitution use the  rule 2.**
5. If $Q = x^m$ $\tbraks{m \ge 0, m \in \Z}$. $$P.I = \frac 1{f(D)} = \tbraks{f(D)}^{-1}x^m$$Now expand using the binomial.
6. If $Q  = e^{ax}v(x)$, $$P.I = \frac 1{f(D)}e^{ax}v = e^{ax}\tbraks{\frac {1}{f(D+a)}v}$$
7. If $f(D) =D^2 + a^2$ . $$P.I = \frac 1 {D^2+a^2} \sin{ax} = \frac{-x}{2a} \cos{ax}$$ $$P.I = \frac 1 {D^2+a^2} \cos{ax} = \frac{x}{2a} \sin{ax}$$
8. If $Q = x^mv(x)$ $$\begin{align}P.I &= \frac{x^m v}{f(D)} \\ &= x^m \frac 1{f(D)}v+ mx^{m-1}\tbraks{\diff{}{D}{}\cdot \frac 1{f(D)}}v + ^mC_2x^{m-2}\tbraks{\diff{}{D}{2}\cdot \frac 1{f(D)}}v + ^mC_3x^{m-3}\tbraks{\diff{}{D}{3}\cdot \frac 1{f(D)}}v + \cdots \end{align}$$ 

## Cauchy-Euler Equation.
$$\summ{i=0}n a_{n-i}x^iD^i = Q$$
Substitution, $x = e^z$ $\implies z = \ln x$.  $(D')^k = \diff{}{z}{k}$, then  $$
\begin{align}
&xD \ra D'\\
&x^2D^2 \ra D'(D'-1) \\
&x^3D^3 \ra D'(D'-1)(D'-2)\\
&\vdots\\
&x^nD^n \ra \prod_{i=0}^{n-1}\fbraks{D-i}
\end{align}
$$
**A special case for Second degree homogeneous equation** 
$$x^2 \diff{y}{x}{2}+ ax\diff{y}{x}{}+by=0$$

Let $y = x^m$(trial solution). 
Rearranging and factoring gives the equation:
$$m^2 +(a-1)m +b =0$$
Three possible cases for roots:
1. 2 distinct solutions, $m_1,m_2$ $$y = c_1 x^{m_1}+c_2 x^{m_2}$$
2. Repeated roots, $$y = (c_1+c_2 \ln x)x^m$$
3. Complex roots, $$y = x^\alpha\fbraks{c_1\cos(\beta\ln x) + c_2 \sin (\beta \ln x)}$$Where $\alpha = \mathfrak{Re}\braces{m}$ and $\beta = \mathfrak{Im}\braces{m}$ 


## Method of variation Parameter
$$\begin{align}
&\diff{y}{x}{2} + P\diff{y}{x}{} + Qy = R \\
\iff &y''+Py'+Qy =R\\
\end{align}$$
Where, $P$ and $Q$ are polynomials in $\R$.  Let $y_1$ and $y_2$ are two solution to the equation. Define Wronskian as:- $$W(y_1,y_2) = \begin{vmatrix} y_1 & y_2 \\ y'_1 & y'_2\end{vmatrix}$$
The general solution can be written as $y = uy_1+v y_2$ , where : 
$$
\begin{matrix}u= \int \frac{-y_2R}{W(y_1,y_2)}dx & v = \int \frac{y_1R}{W(y_1,y_2)}dx\end{matrix}
$$
Note:- $W(y_1,y_2) \neq 0 \implies$ $y_1$ and $y_2$ are linearly independent.
### For homogeneous Linear 2nd order

$$y''+Py'+Qy=0$$
1.  $W(y_1,y_2) \neq 0 \implies$ $y_1$ and $y_2$ are linearly independent.
2. $W(y_1,y_2) = 0 \implies$ $y_1$ and $y_2$ are linearly dependent.
3. $W(y_1, y_2) =C e^{-\int_{x_0}^x P dx}$  , $x_0, x \in I \subset \R$ .