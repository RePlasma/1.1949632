# Analytical results for a Fokker–Planck equation in the small noise limit

Author of paper: Eric Lutz

Link to paper: https://pubs.aip.org/aapt/ajp/article/73/10/968/1042378/Analytical-results-for-a-Fokker-Planck-equation-in

Notebook by: [Óscar Amaro](https://github.com/OsAmaro) (2023)

Abstract: _We present analytical results for the lowest order cumulants of a stochastic process described by a Fokker–Planck equation with nonlinear drift, which appears in the description of laser cooling of atoms. We show that, in the limit of small fluctuations, the mean, the variance, and the covariance of the process can be expressed in compact form with the help of the Lambert function. As an application, we discuss the interplay of noise and nonlinearity far from equilibrium._



### Proof of deterministic solution $\bar{v}(t)$

Assuming solution eq 7: $v = \sqrt{W[T]}$ with $W=W[T]$ and $T=e^{-2t+C}$, we have

$$\dfrac{dv}{dT} = \dfrac{1}{2} \dfrac{W'}{\sqrt{W}} = \dfrac{dv}{dt} \dfrac{dt}{dT} = -\dfrac{\dot{v}}{2 T}$$

because $dT/dt=-2T$, so $\dot{v} = -T ~W' / \sqrt{W}$. On the other hand, since $\dot{v} = -v/(1+v^2)$ from eq 4, we have

$$-T \dfrac{W'}{\sqrt{W}} = - \dfrac{\sqrt{W}}{1+W} \implies W' = \dfrac{W}{T(1+W)}$$

which is precisely the differential equation that the Lambert function satisfies (see https://en.wikipedia.org/wiki/Lambert_W_function).
