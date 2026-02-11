**标签：** #RL/mechanism
**来源：**https://arxiv.org/abs/2507.07969

--- 
## 正文 
![[截屏2026-02-09 13.47.12.png]]
two styles:
1. standard(open-loop): 
![[截屏2026-02-09 13.48.12.png]]
![[截屏2026-02-09 13.48.23.png]]
2. Planning(closed-loop): Actor produce action chunk but only one action is performed at each iteration, Q is updated with "sampled action chunk" which is likely to contain different planned actions.



## 关联链接 

Decoupling Q and Actor: [[Decoupled Q-chunking]]
