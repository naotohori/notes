
# Derivation of the Debye-Huckel potential [^RobinsonBook]

Poisson's equation is

$$\nabla^{2}\phi(r)=-\frac{1}{\varepsilon}\rho(r).$$

In case of spherical symmetry,

$$
\nabla^{2}=\frac{1}{r^{2}}\frac{d}{dr}\left(r^{2}\frac{d}{dr}\right)
$$

(In general, $$\nabla^{2}=\frac{1}{r^{2}}\frac{\partial}{\partial r}\left(r^{2}\frac{\partial}{\partial r}\right)+\frac{1}{r^{2}\sin\theta}\frac{\partial}{\partial\theta}\left(\sin\theta\frac{\partial}{\partial\theta}\right)+\frac{1}{r^{2}\sin^{2}\theta}\frac{\partial^{2}}{\partial\phi^{2}}$$)

$$
\frac{1}{r^{2}}\frac{d}{dr}\left(r^{2}\frac{d}{dr}\right)\phi(r)=-\frac{1}{\varepsilon}\rho(r)
$$

Because of the electric neutrality, 

$$
\sum_{i=1}^{s}n_{i}z_{i}=0
$$

where $$n_{i}$$ is the average number per unite volume of ion type
$$i$$, and $$z_{i}$$ is the valence value.

$$
\int_{a}^{\infty}4\pi r^{2}\rho_{j}dr=-z_{j}e
$$

$$
n_{i}^{\prime}=n_{i}\exp\left(-\frac{z_{i}e\phi_{j}}{kT}\right)
$$

$$\begin{align*}
\rho_{j} & =\sum_{i}n_{i}z_{i}e\exp\left(-\frac{z_{i}e\phi_{j}}{kT}\right)\\
 & =\sum n_{i}z_{i}e-\sum n_{i}z_{i}e\left(\frac{z_{i}e\phi_{j}}{kT}\right)+\sum\frac{n_{i}z_{i}e}{2}\left(\frac{z_{i}e\phi_{j}}{kT}\right)-\cdots
\end{align*}$$

If $$z_{i}e\phi_{j}\ll kT$$,

$$
\rho_{j}\approx-\sum_{i=1}^{s}\frac{n_{i}z_{i}^{2}e^{2}\phi_{j}}{kT}
$$

$$
\begin{eqnarray*}
\frac{1}{r^{2}}\frac{d}{dr}\left(r^{2}\frac{d\phi_{j}}{dr}\right) & = & \frac{e^{2}}{\varepsilon kT}\sum_{i}n_{i}z_{i}^{2}\phi_{j}\\
 & = & \kappa^{2}\phi_{j}
\end{eqnarray*}
$$

$$
\kappa^{2}=\frac{e^{2}\sum n_{i}z_{i}^{2}}{\varepsilon kT}
$$

$$u=r\phi_{j}(r)$$

$$
\begin{eqnarray*}
\frac{1}{r^{2}}\frac{d}{dr}\left(r^{2}\frac{d\phi_{j}}{dr}\right) & = & \frac{1}{r^{2}}\frac{d}{dr}\left(r^{2}\frac{d}{dr}(ur^{-1})\right)\\
 & = & \frac{1}{r^{2}}\frac{d}{dr}\left(r^{2}\left(r^{-1}\frac{du}{dr}-r^{-2}u\right)\right)\\
 & = & \frac{1}{r^{2}}\frac{d}{dr}\left(r\frac{du}{dr}-u\right)\\
 & = & \frac{1}{r^{2}}\left(\frac{du}{dr}+r\frac{d^{2}u}{dr^{2}}-\frac{du}{dr}\right)\\
 & = & \frac{1}{r}\frac{d^{2}u}{dr^{2}}
\end{eqnarray*}
$$

$$
\frac{d^{2}u}{dr^{2}}=\kappa^{2}u
$$

$$
u=Ae^{-\kappa r}+Be^{\kappa r}
$$

$$
\phi_{j}(r)=A\frac{e^{-\kappa r}}{r}+B\frac{e^{\kappa r}}{r}
$$

$$\phi_{j}$$ should not be infinite when $$r\gg1$$, so $$B=0$$.

$$
\begin{eqnarray*}
\rho_{j}(r) & = & -A\frac{e^{-\kappa r}}{r}\sum_{i}\frac{n_{i}z_{i}e^{2}}{kT}\\
 & = & -A\frac{e^{-\kappa r}}{r}\varepsilon\kappa^{2}
\end{eqnarray*}
$$

$$
\begin{eqnarray*}
\int_{a}^{\infty}4\pi r^{2}\left(-A\frac{e^{-\kappa r}}{r}\varepsilon\kappa^{2}\right)dr & = & -z_{j}e\\
4\pi A\kappa^{2}\varepsilon\int_{a}^{\infty}re^{-\kappa r}dr & = & z_{j}e\\
4\pi A\kappa^{2}\varepsilon\left(\left[-\frac{1}{\kappa}re^{-\kappa r}\right]_{a}^{\infty}+\left[-\frac{1}{\kappa^{2}}e^{-\kappa r}\right]_{a}^{\infty}\right) & = & z_{j}e\\
4\pi A\kappa^{2}\varepsilon\left(\frac{1}{\kappa}ae^{-\kappa a}+\frac{1}{\kappa^{2}}e^{-\kappa a}\right) & = & z_{j}e\\
4\pi A\varepsilon e^{-\kappa a}\left(\kappa a+1\right) & = & z_{j}e\\
A & = & \frac{z_{j}e}{4\pi\varepsilon\left(\kappa a+1\right)}e^{\kappa a}
\end{eqnarray*}
$$

$$
\phi_{j}(r)=\frac{z_{j}e}{4\pi\varepsilon}\frac{e^{\kappa a}}{1+\kappa a}\frac{e^{-\kappa r}}{r}
$$

$$
\kappa=\sqrt{\frac{e^{2}\sum n_{i}z_{i}^{2}}{\varepsilon kT}}
$$

If $$\kappa a\ll1$$, then $$\frac{e^{\kappa a}}{1+\kappa a}\approx1$$

$$
\phi_{j}(r)=\frac{z_{j}e}{4\pi\varepsilon}\frac{e^{-\kappa r}}{r}
$$

[^RobinsonBook]: R.A. Robinson & R.H. Stokes, Electrolyte Solutions, 2nd ed. (2002)
