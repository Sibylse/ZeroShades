---
layout: single
title:  "The Descent Lemma"
date:   2021-08-25
mathjax: true
subtitle: The inverse Lipschitz constant as stepsize
hidden: true
---
The descent lemma is _the_ reason why the inverse Lipschitz constant of the gradient gives us a good stepsize. It goes as follows:     
*Descent Lemma*    
Let $f:\mathdd{R}^d\rightarrow \mathbb{R}$ be a continously differentiable function whose gradient $\nabla f$ is Lipschitz continuous with constant $L$. Then,
\[f(x+y)\leq f(x)+y^\top\nabla f(x) +\frac{L}{2}\lVert y\rVert^2.\]
_Proof_: We denote with $g(\alpha)=f(x+\alpha y)$. Then we have:
$$
\begin{align*}
f(x+y)-f(x) &= g(1)-g(0)\\
&= \int_0^1 \frac{dg(\alpha)}{d\alpha} d\alpha\\
&= \int_0^1 \frac{d}{d\alpha} f(x+\alpha y)d\alpha\\
&= \int_0^1 y^\top \nabla f(x+\alpha y)d\alpha\\
&= \int_0^1 y^\top \nabla f(x+\alpha y) -y^\top +y^\top\nabla f(x)d\alpha\\
&\leq \left\lvert \int_0^1 y^\top(\nabla f(x+\alpha y)-\nabla f(x))d\alpha\right\rvert + \int_0^1y^\top\nabla f(x)d\alpha\\
&\leq \int_0^1\lVert y\rVert\lVert\nabla f(x+\alpha y)-\nabla f(x)\rVertd\alpha + y^\top\nabla f(x)\\
&\leq \lVert y\rVert L\int_0^1 \lVert x+\alpha y-x\rVert d\alpha + y^\top\nabla f(x)\\
&= \lVert y\rVert^2 L\frac12 + y^\top\nabla f(x)
\end{align*}
$$
From the descent lemma follows that using a stepsize $\alpha < \frac{2}{L}$ results in a guaranteed decrease of gradient descent steps. 
This is because we have according to the descent lemma we have
$$
\begin{align*}
f(x-\alpha\nabla f(x))&\leq f(x) -\alpha\lVert \nabla f(x)\rVert^2 + \frac{L}{2}\lVert y\rVert^2\\
&= f(x)+\alpha\left(\frac{L}{2}\alpha - 1\right)\lVert \nabla f(x)\rVert^2
\end{align*}
$$
From the last inequality follows that we decrease the objective with every gradient descent step if $\alpha<\frac{L}{2}$.
