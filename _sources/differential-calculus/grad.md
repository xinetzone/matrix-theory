# 微分

有矩阵 $\mathbf{A} = [\mathbf{a}_1, \mathbf{a}_2, \cdots, \mathbf{a}_m]^{\top} \in \mathbb{R}^{m \times n}$、向量 $\mathbf{x} = [x_1, x_2, \cdots, x_n]^{\top} \in \mathbb{R}^{n}$ 和 $\mathbf{y} = [y_1, y_2, \cdots, y_m]^{\top} \in \mathbb{R}^{m}$，令：

$$
\begin{aligned}
\mathbf{f}:\; &\mathbb{R}^n \to \mathbb{R}^m\\
&\mathbf{x} \longmapsto \mathbf{y}
\end{aligned}
$$

记 $\mathbf{f} = (f_1, f_2, \cdots, f_m)^{\top}$，其中： 

$$
\begin{aligned}
f_i:\; &\mathbb{R}^n \to \mathbb{R}\\
&\mathbf{x} \longmapsto y_i
\end{aligned}
$$

则有：

$$
\mathbf{df} = [\mathbf{d}f_1, \mathbf{d} f_2, \cdots, \mathbf{d} f_m]^{\top}
$$

$$
\mathbf{Ax} = \begin{bmatrix}
   \langle \mathbf{a}_1, \mathbf{x} \rangle\\
   \langle \mathbf{a}_2, \mathbf{x} \rangle\\
   \vdots \\
   \langle \mathbf{a}_m, \mathbf{x} \rangle
\end{bmatrix}
$$

## $\nabla$ 定义

参考：[Del - Wikipedia](https://en.wikipedia.org/wiki/Del)

易知 $\{\mathbf{d} x_1, \mathbf{d} x_2, \cdots, \mathbf{d} x_n\}$，$\{\mathbf{d} y_1, \mathbf{d} y_2, \cdots, \mathbf{d} y_m\}$ 分别为 $\mathbb{R}^n$ 和 $\mathbb{R}^m$ 的一组标准正交基，则记微分算子：

$$
\nabla_{\mathbf{x}} = (\frac{\partial}{\partial x_1}, \frac{\partial}{\partial x_2}, \cdots, \frac{\partial}{\partial x_n})^{\top},
$$

同样，也有：

$$
\nabla_{\mathbf{y}} = (\frac{\partial}{\partial y_1}, \frac{\partial}{\partial y_2}, \cdots, \frac{\partial}{\partial y_m})^{\top},
$$

则有

$$
\begin{cases}
\mathbf{dy}_i = \frac{\partial f_i(\mathbf{x})}{ \partial x_i} x_i
\end{cases}
$$

记微分导数：

$$
\frac{\partial \mathbf{f}} {\partial \mathbf{x}} = \mathbf{f}^{'}(\mathbf{x}) = \nabla \mathbf{f} = \frac{\partial (f_1, f_2, \cdots, f_m)} {\partial (x_1, x_2, \cdots, x_n)}
$$

这样，有：

$$
\mathbf{d} \mathbf{y} = \nabla_{\mathbf{x}}(\mathbf{y}) = \mathbf{f}^{'}(\mathbf{x}) \nabla_{\mathbf{x}} = 
$$