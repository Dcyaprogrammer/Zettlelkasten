**标签：** #DL/GenerativeModel 
**来源：**

--- 
## 正文 

A type of [[Auto-Encoders]]

pair data: clean and corrupted

![[截屏2026-02-10 00.20.23.png]]
output denoised version, trained to approach clean version

possible issue: this should has a condition on noisy input here
![[截屏2026-02-10 00.20.51.png]]

![[截屏2026-02-10 00.23.07.png]]

since we use MSE loss, the optimized denoising ae is actutally
$$D^*(\tilde{x}) = \mathbb{E}[x | \tilde{x}]$$
and [[Tweedie's formula]] tells us
$$\mathbb{E}[x | \tilde{x}] = \tilde{x} + \sigma^2 \nabla_{\tilde{x}} \log p(\tilde{x})$$
$$D^*(\tilde{x}) \approx \tilde{x} + \sigma^2 \nabla_{\tilde{x}} \log p(\tilde{x})$$

So denoising ae essentially learns the score function of noisy distribution
## 关联链接 
https://www.youtube.com/watch?v=0V96wE7lY4w
[[VAE]]
[[DDPM]] 
