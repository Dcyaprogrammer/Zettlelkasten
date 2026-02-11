**标签：**  #ML #Math 
**来源：** 

--- 
## 正文

$P(x)$ : evidence, data distribution
$P(z|x)$: posterior of latent variable $z$, this posterior is hard to compute
so we use $q(z)$ to model posterior

$D_{KL}(q||p)$ = $E_q[log\frac{q(z)}{p(z|x)}]$ 
		= $E_q[logq(z)]+E_q[log(p(x))]-E_q[logp(x,z)]$
		
Then we have
$logp(x)$ = $D_{KL}(q||p)$ + **$E_q[logp(x,z)]$ - $E_q[logq(z)]$**
Since we have $D_{KL}\geq0$ , then maximize $p(x)$ is equivalent to minimize KL, and the latter part is the ELBO(evidence lower bound)



## 关联链接 
VI family:
[[Stein Variational Gradient Decent]]


