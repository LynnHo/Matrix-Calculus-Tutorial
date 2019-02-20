<h1> <p align="center"> Examples </p> </h1>

<!-- MarkdownTOC -->

- [1. Actual Examples](#1-actual-examples)
- [2. Abstract Examples](#2-abstract-examples)

<!-- /MarkdownTOC -->

## 1. Actual Examples

## 2. Abstract Examples

**E.g. 1**, $\frac{d(z(\mathbf{y}(\mathbf{X})))}{d\mathbf{X}}$, ($\mathbf{X}$ is a $p\times q$ matrix),

\begin{align*}
\frac{dz}{d\mathbf{X}}&=
\begin{bmatrix}
\frac{\partial z}{\partial x_{11}} & \frac{\partial z}{\partial x_{21}} & \cdots & \frac{\partial z}{\partial x_{p1}}\\
\frac{\partial z}{\partial x_{12}} & \frac{\partial z}{\partial x_{22}} & \cdots & \frac{\partial z}{\partial x_{p2}}\\
\vdots                             & \vdots                             & \ddots & \vdots\\
\frac{\partial z}{\partial x_{1q}} & \frac{\partial z}{\partial x_{2q}} & \cdots & \frac{\partial z}{\partial x_{pq}}\\
\end{bmatrix}\\
&=
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{11}} & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{21}} & \cdots & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{p1}}\\
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{12}} & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{22}} & \cdots & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{p2}}\\
\vdots                                                                            & \vdots                                                                            & \ddots & \vdots\\
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{1q}} & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{2q}} & \cdots & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{pq}}\\
\end{bmatrix}\\
&=
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{:1}}\\
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{:2}}\\
\vdots\\
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{:q}}\\
\end{bmatrix}\\
&=
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{y}} & \mathbf{0}                             & \cdots & \mathbf{0}\\
\mathbf{0}                             & \frac{\partial z}{\partial \mathbf{y}} & \cdots & \mathbf{0}\\
\vdots                                 & \vdots                                 & \ddots & \vdots\\
\mathbf{0}                             & \mathbf{0}                             & \cdots & \frac{\partial z}{\partial \mathbf{y}}   \\
\end{bmatrix}
\begin{bmatrix}
\frac{\partial \mathbf{y}}{\partial x_{:1}}\\
\frac{\partial \mathbf{y}}{\partial x_{:2}}\\
\vdots\\
\frac{\partial \mathbf{y}}{\partial x_{:q}}\\
\end{bmatrix}\\
&=
(\mathbf{I}_{q\times q}\otimes \frac{\partial z}{\partial \mathbf{y}})
\begin{bmatrix}
\frac{\partial \mathbf{y}}{\partial x_{:1}}\\
\frac{\partial \mathbf{y}}{\partial x_{:2}}\\
\vdots\\
\frac{\partial \mathbf{y}}{\partial x_{:q}}\\
\end{bmatrix},
\end{align*}

or

\begin{align*}
\frac{dz}{d\mathbf{X}} &=
\begin{bmatrix}
\frac{\partial z}{\partial x_{11}} & \frac{\partial z}{\partial x_{21}} & \cdots & \frac{\partial z}{\partial x_{p1}}\\
\frac{\partial z}{\partial x_{12}} & \frac{\partial z}{\partial x_{22}} & \cdots & \frac{\partial z}{\partial x_{p2}}\\
\vdots                             & \vdots                             & \ddots & \vdots\\
\frac{\partial z}{\partial x_{1q}} & \frac{\partial z}{\partial x_{2q}} & \cdots & \frac{\partial z}{\partial x_{pq}}\\
\end{bmatrix}\\
&=
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{11}} & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{21}} & \cdots & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{p1}}\\
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{12}} & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{22}} & \cdots & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{p2}}\\
\vdots                                                                            & \vdots                                                                            & \ddots & \vdots\\
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{1q}} & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{2q}} & \cdots & \frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{pq}}\\
\end{bmatrix}\\
&=
\begin{bmatrix}
(\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{1:}})^\top&
(\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{2:}})^\top&
\cdots&
(\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{p:}})^\top
\end{bmatrix}\\
&=
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{1:}}\\
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{2:}}\\
\vdots\\
\frac{\partial z}{\partial \mathbf{y}}\frac{\partial \mathbf{y}}{\partial x_{p:}}
\end{bmatrix}^\top\\
&=
((\mathbf{I}_{p\times p}\otimes \frac{\partial z}{\partial \mathbf{y}})
\begin{bmatrix}
\frac{\partial \mathbf{y}}{\partial x_{1:}}\\
\frac{\partial \mathbf{y}}{\partial x_{2:}}\\
\vdots\\
\frac{\partial \mathbf{y}}{\partial x_{p:}}\\
\end{bmatrix})^\top.
\end{align*}

In the above, we haven't used any differential technique, because we haven't defined the derivative of vector-by-matrix $\frac{d \mathbf{y}}{d\mathbf{X}}$ which could be a 3D tensor. However, in some cases such as $\mathbf{y}=\mathbf{W}\mathbf{x}$ (w.r.t. $\mathbf{W}$), the differential technique still works (see [this example](./README.md#y=Wx)).

**E.g. 2**, $\frac{d(z(\mathbf{Y}(\mathbf{X})))}{d\mathbf{X}}$, ($\mathbf{Y}$ is a $m\times n$ matrix and $\mathbf{X}$ is a $p\times q$ matrix),

\begin{align*}
\frac{dz}{d\mathbf{X}} &=
\begin{bmatrix}
\frac{\partial z}{\partial x_{11}} & \frac{\partial z}{\partial x_{21}} & \cdots & \frac{\partial z}{\partial x_{p1}}\\
\frac{\partial z}{\partial x_{12}} & \frac{\partial z}{\partial x_{22}} & \cdots & \frac{\partial z}{\partial x_{p2}}\\
\vdots                             & \vdots                             & \ddots & \vdots\\
\frac{\partial z}{\partial x_{1q}} & \frac{\partial z}{\partial x_{2q}} & \cdots & \frac{\partial z}{\partial x_{pq}}\\
\end{bmatrix}\\
&=
\begin{bmatrix}
\mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{11}})\mathbf{1}_{n} & \mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{21}})\mathbf{1}_{n} & \cdots & \mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{p1}})\mathbf{1}_{n}\\
\mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{12}})\mathbf{1}_{n} & \mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{22}})\mathbf{1}_{n} & \cdots & \mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{p2}})\mathbf{1}_{n}\\
\vdots & \vdots & \ddots & \vdots\\
\mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{1q}})\mathbf{1}_{n} & \mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{2q}})\mathbf{1}_{n} & \cdots & \mathbf{1}_{m}^\top(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{pq}})\mathbf{1}_{n}\\
\end{bmatrix}\\
&=
\begin{bmatrix}
\mathbf{1}_{m}^\top\small
\begin{bmatrix}
(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{11}})\mathbf{1}_{n} & (\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{21}})\mathbf{1}_{n} & \cdots & (\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{p1}})\mathbf{1}_{n}\\
\end{bmatrix}\\
\mathbf{1}_{m}^\top\small
\begin{bmatrix}
(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{12}})\mathbf{1}_{n} & (\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{22}})\mathbf{1}_{n} & \cdots & (\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{p2}})\mathbf{1}_{n}\\
\end{bmatrix}\\
\vdots\\
\mathbf{1}_{m}^\top\small
\begin{bmatrix}
(\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{1q}})\mathbf{1}_{n} & (\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{2q}})\mathbf{1}_{n} & \cdots & (\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{pq}})\mathbf{1}_{n}\\
\end{bmatrix}
\end{bmatrix}\\
&=
\begin{bmatrix}
\mathbf{1}_{m}^\top\small
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{11}} & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{21}} & \cdots & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{p1}}\\
\end{bmatrix}
(\mathbf{I}_{p\times p}\otimes \mathbf{1}_{n})\\
\mathbf{1}_{m}^\top\small
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{12}} & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{22}} & \cdots & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{p2}}\\
\end{bmatrix}
(\mathbf{I}_{p\times p}\otimes \mathbf{1}_{n})\\
\vdots\\
\mathbf{1}_{m}^\top\small
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{1q}} & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{2q}} & \cdots & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{pq}}\\
\end{bmatrix}
(\mathbf{I}_{p\times p}\otimes \mathbf{1}_{n})
\end{bmatrix}\\
&=
(\mathbf{I}_{q\times q}\otimes \mathbf{1}_{m}^\top)
\begin{bmatrix}
\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{11}} & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{21}} & \cdots & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{p1}}\\
\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{12}} & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{22}} & \cdots & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{p2}}\\
\vdots\\
\frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{1q}} & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{2q}} & \cdots & \frac{\partial z}{\partial \mathbf{Y}^\top}\circ\frac{\partial\mathbf{Y}}{\partial x_{pq}}
\end{bmatrix}
(\mathbf{I}_{p\times p}\otimes \mathbf{1}_{n})\\
&=
(\mathbf{I}_{q\times q}\otimes \mathbf{1}_{m}^\top)
((\mathbf{1}_{q\times p}\otimes \frac{\partial z}{\partial \mathbf{Y}^\top})\circ\begin{bmatrix}
\frac{\partial\mathbf{Y}}{\partial x_{11}} & \frac{\partial\mathbf{Y}}{\partial x_{21}} & \cdots & \frac{\partial\mathbf{Y}}{\partial x_{p1}}\\
\frac{\partial\mathbf{Y}}{\partial x_{12}} & \frac{\partial\mathbf{Y}}{\partial x_{22}} & \cdots & \frac{\partial\mathbf{Y}}{\partial x_{p2}}\\
\vdots\\
\frac{\partial\mathbf{Y}}{\partial x_{1q}} & \frac{\partial\mathbf{Y}}{\partial x_{2q}} & \cdots & \frac{\partial\mathbf{Y}}{\partial x_{pq}}
\end{bmatrix})
(\mathbf{I}_{p\times p}\otimes \mathbf{1}_{n}).
\end{align*}

In the above, we haven't used any differential technique, because we haven't defined the derivative of matrix-by-matrix $\frac{d \mathbf{Y}}{d\mathbf{X}}$ which could be a 4D tensor. However, in some cases such as $\mathbf{Y}=\mathbf{A}\mathbf{X}$, the differential technique still works (see [this example](./README.md#Y=AX)).