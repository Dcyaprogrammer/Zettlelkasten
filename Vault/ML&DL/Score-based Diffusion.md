**标签：**  #DL/GenerativeModel 
**来源：** https://arxiv.org/pdf/2011.13456

--- 
## 正文 

Consider [[DDPM]] in continuous time:
we essentially get a [[Ito's formula]] which will converge any init distribution into a normal Gaussian

![[截屏2026-02-11 22.38.16.png]]

Thus we can reverse the SDE to generate image
The reverse SDE:
![[截屏2026-02-11 22.39.36.png]]
Since the score function is unknown, we have to use NN to approximate(Score matching)
Objective(viable):
![[截屏2026-02-11 22.41.06.png]]
Now we can run the SDE!
For actual implementation we need to discretize the SDE:
Using [[Euler-Maruyama Discretization]] 

![[截屏2026-02-11 22.42.24.png]]
## 关联链接 
https://www.youtube.com/watch?v=lUljxdkolK8
