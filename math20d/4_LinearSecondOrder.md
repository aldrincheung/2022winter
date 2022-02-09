# Chapter 4: Linear Second-Order Differential Equation

### 4.2: Homogenus Linear Equations: General Solution
- To solve: $\quad ay''+by'+cy=0$
- Because the derivates are multiple of each other, the most possible form of y(x) is $e^{rt}$
  - $ar^2e^{rt}+bre^{rt}+ce^{rt}=0$
  - $e^{rt}(ar^2+br+c)=0$
  - $(ar^2+br+c)=0$ $\quad\quad \to\quad r=\cfrac{-b\pm\sqrt{b^2-4ac}}{2a}$
- single roots: $\quad y(t)=c_1e^{r_1t}+c_2e^{r_2t}$
- repeated root: $\quad y(t)=c_1e^{rt}+c_2te^{rt}$

<br/>

### 4.3: Auxiliary Equations with Complex Roots
- In the case where $b^2-4ac<0$, $\quad\quad r=\alpha\pm i\beta=- \cfrac{b}{2a}\pm i \cfrac{\sqrt{4ac-b^2}}{2a}$
- $e^{rt}=e^{(\alpha +i\beta)t}=e^{\alpha t}e^{i\beta t}$
  - $e^{i\theta} =1+(i\theta)+\cfrac{(i\theta)^2}{2!}+\cdots+\cfrac{(i\theta)^n}{n!}+\cdots=\left( 1-\cfrac{\theta^2}{2!}+\cfrac{\theta^4}{4!}+\cdots \right)+i\left( \theta - \cfrac{\theta^3}{3!} + \cfrac{\theta^5}{5!} + \cdots\right)$
  - $\cos\theta = 1-\cfrac{\theta^2}{2!} + \cfrac{\theta^4}{4!} + \cdots$
  - $\sin\theta = \theta - \cfrac{\theta^3}{3!} + \cfrac{\theta^5}{5!} + \cdots$
  - $\therefore e^{i\theta} = \cos\theta + i\sin\theta$
  - $\therefore e^{(\alpha + i \beta)t} = e^{\alpha t}(\cos\beta t+i\sin\beta t)$
  - $\therefore y(t)=c_1e^{\alpha t}(\cos\beta t+\sin\beta t)+c_2e^{\alpha t}(\cos\beta t-\sin\beta t)$
- $y(t)=c_1e^{\alpha t}\cos\beta t + c_2e^{\alpha t}\sin\beta t$

<br/>

### 4.4 Nonhomogeneous Equations: The Method of Undetermined Coefficients
- "judicious guessing" to derive solution of: $ay''+by'+cy=f(t)$
  
|f(t) | Guess | Name |
|---|---|---|
|$3t$ | $y(t)=At+B$ ||
|$Ct^m$| $y_p(t)=A_mt^m+\cdots+A_1t+A_0$|method of undetermined coefficients|
|$Ce^{mt}$| $y_p(t)=Ae^{mt}$||
|$\sin t$| $y_p(t)=A\sin t+B\cos t$|
|$Ct^me^{nt}$|$y_p(t)=(A_mt^m+\cdots+A_1t+A_0)e^{nt}$|

- Method of Undetermined Coefficients

|f(t) | solution in the form of:|
|---|---|
|$Ct^me^{rt}$|$y_p(t)=t^s(A_mt^m+\cdots+A_1t+A_0)e^{rt}$<br/><br/>i) $s=0$ if r is not a root of the associated auxiliary equation<br/>ii) $s=1$ if r is a simple root of the associated auxiliary equation<br/>iii) $s=2$ if r is a double root of the associated auxiliary equation|
|$Ct^me^{\alpha t}\cos\beta t$<br/>or<br/>$Ct^me^{\alpha t}\sin\beta t$|$y_p(t)=t^s(A_mt^m+\cdots+A_1t+A_0)e^{\alpha t}\cos\beta t+t^s(B_mt^m+\cdots+B_1t+B_0)e^{\alpha t}\sin\beta t$<br/><br/>i) $s=0$ if r is not a root of the associated auxiliary equation<br/>ii) $s=1$ if r is a root of the associated auxiliary equation|