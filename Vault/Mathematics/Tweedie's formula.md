**标签：**  #Math #DL 
**来源：**

--- 
## 正文 

假设 $\tilde{x} = x + \epsilon$，其中噪声 $\epsilon \sim \mathcal{N}(0, \sigma^2 I)$。

Tweedie 公式告诉我们，**真实信号的后验均值**可以用**观察数据的边缘分布的梯度**（Score）来表示：

$$\mathbb{E}[x | \tilde{x}] = \tilde{x} + \sigma^2 \nabla_{\tilde{x}} \log p(\tilde{x})$$

- $\tilde{x}$: 你看到的加噪图像。
    
- $\nabla_{\tilde{x}} \log p(\tilde{x})$: 数据密度函数的梯度（Score Function）。这指引着从“低密度区域”指向“高密度区域”的方向


## 关联链接 
[[Denoising-Autoencoders]]
