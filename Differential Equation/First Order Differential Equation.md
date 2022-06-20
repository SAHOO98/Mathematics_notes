

# Types of DE
## Homogenous form
$$\diff yx{} = \frac {f_1(x,y)}{f_2(x,y)}$$Here both $f_1$ and $f_2$ are [[Homogenous fucntion]] of same order \ degree. Then, let $\frac yx =v \implies \diff yx{} = v +x \diff vx{}$. Therefore above equation  transforms to $$\diff yx{} = f\left(\frac yx\right) \implies v + x\diff vx{} = f(v) \implies \frac {dv}{-v+f(v)}=\frac{dx}{x}$$
## Linear DE of first order 
### Standard Form
$$\diff yx{} + P(x)y = Q(x)$$
$$I.F = e^{\int P\cdot dx}$$
**Solution**: $y(I.F) = \int Q\cdot (I.F) dx +c$. 

### Other Form
$$\diff xy{} + P(y)x = Q(y)$$
$$I.F = e^{\int P\cdot dy}$$
## Bernoullie's Linear DE
$$\diff yx{} + P(x)y = Q(x)y^n$$
**Substitution**: 
$y^{1-n} = v$ then $(1-n)y^{-n} \diff yx{} = \diff vx{}$ . Therefore,
$$ \begin{align*} 
&\diff vx {}+ (1-n)Pv = (1-n)Q \\
\implies & \diff vx{} +P' v = Q' \\
I.F&= e^{\int P' dx}
\end{align*} 
$$
and the rest continues as usual.
##  Exact DE 
$$Mdx+Ndy=0$$
If $$\pdiff{M}{y} = \pdiff{N}{x}$$ then the above de is in Exact form.

**Solution** : $$\int_{\text{y as constant}} M dx + \int_{\text{free from x terms}} Ndy = C$$
## Reducible to exact DE and Integrating factor(I.F)
If DE is not in *exact form* then multiplying a I.F will turn the equation to a *exact DE*. Following the ways to calculate I.F :
* By Inspection:
	1. $xdy+ydx = d(xy)$
	2. $xdy-ydx \implies I.F = \frac1{x^2}$
	3. $xdy-ydx \implies I.F = \frac1{x^2}$
* If $M(x,y)$ and $N(x,y)$  are homogeneous then $I.F = \frac1{Mx+Ny}$ such that $Mx+Ny \neq0$.
* If the DE is in form $$f_1(xy)dx+f_2(xy)dy=0$$ and $Mx-Ny\neq0$ then $I.F = \frac1{Mx-Ny}$
* If $$\frac1N \left(\pdiff My - \pdiff Nx\right)=f(x)$$ then $I.F  = e^{\int f(x) dx}$
* If $$\frac1M \left(\pdiff My -\pdiff Nx\right)=-f(y)$$ then $I.F= e^{\int -f(y) dy}$


 