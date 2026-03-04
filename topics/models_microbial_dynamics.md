
## Common models Inactivation
### Weibull distribution

It models a broad range of random variables, largely in the nature of a time to failure or time between events. Examples are maximum one-day rainfalls and the time a user spends on a web page.
$$ f(x;\lambda,k) = \begin{cases} \dfrac{k}{\lambda}\left(\dfrac{x}{\lambda}\right)^{k-1} e^{-(x/\lambda)^{k}}, & x \ge 0, \\ 0, & x < 0. \end{cases} $$
where k > 0 is the shape parameter and λ > 0 is the scale parameter of the distribution. If the quantity, x, is a "time-to-failure", the Weibull distribution gives a distribution for which the failure rate is proportional to a power of time. 

The accumulative form is
$$ F(x;\lambda,k)= \begin{cases} 1 - e^{-(x/\lambda)^k}, & x \ge 0,\\[6pt] 0, & x < 0. \end{cases} $$
Therefore the survivals (N/N0) is the 1-CDF therefore
$$N=N_0 e^{-(t/\lambda)^k}$$
Where the dynamcis are
$$ \frac{dN}{dt} = -\,\frac{k}{\lambda}\left(\frac{t}{\lambda}\right)^{k-1} N $$


## LogLogistic distribution

( #to-revise ) The log-logistic distribution is widely used to model times to failure, times between events, and biological inactivation times. It is particularly suitable when the hazard rate first increases and then decreases, producing a sigmoidal survival curve. If a positive random variable $t$ follows a Log-Logistic distribution with shape parameter $\beta > 0$ and scale parameter $\alpha > 0$, its probability density function (pdf) is $$ f(t;\alpha,\beta) = \begin{cases} \displaystyle \frac{\beta}{\alpha} \left(\frac{t}{\alpha}\right)^{\beta - 1} \left[ 1 + \left( \frac{t}{\alpha} \right)^{\beta} \right]^{-2}, & t \ge 0, \\[10pt] 0, & t < 0 . \end{cases} $$ The cumulative distribution function (CDF) is $$ F(t;\alpha,\beta) = \frac{1}{1 + \left(\frac{t}{\alpha}\right)^{-\beta}} = \begin{cases} \displaystyle \frac{(t/\alpha)^{\beta}}{1 + (t/\alpha)^{\beta}}, & t \ge 0, \\[10pt] 0, & t < 0 . \end{cases} $$ Therefore, the survival function (the fraction of individuals that remain un‑inactivated at time $t$) is $$ S(t) = 1 - F(t;\alpha,\beta) = \frac{1}{1 + \left( \frac{t}{\alpha} \right)^{\beta}}. $$ If $N(t)$ denotes the surviving population and $N_0$ the initial population size, then $$ N(t) = N_0\,S(t) = \frac{N_0}{1 + \left(\frac{t}{\alpha}\right)^{\beta}}. $$ The corresponding dynamics follow from differentiating the survival law. Since $N(t) = N_0 S(t)$, we obtain $$ \frac{dN}{dt} = N_0\,\frac{dS}{dt} = -\,N_0\, \frac{\beta}{\alpha} \left(\frac{t}{\alpha}\right)^{\beta - 1} \left[ 1 + \left(\frac{t}{\alpha}\right)^{\beta} \right]^{-2}. $$ Thus the rate of inactivation at time $t$ is $$ \frac{dN}{dt} = -\,\frac{\beta}{\alpha} \left(\frac{t}{\alpha}\right)^{\beta - 1} \left[ 1 + \left(\frac{t}{\alpha}\right)^{\beta} \right]^{-2} \, N_0. $$In [Aspridou_2019](../posts/Aspridou_2019.md), each inactivation time follows $t_i \sim \mathrm{LogLogistic}(45.957,\; 2.8583), \qquad i = 1,2,3,\ldots, N,$ and in the ranked‑based nonparametric representation used in the model, the empirical survival at each recorded time is $N(t_i) = N_0\,\mathrm{Rank}(t_i).$
#to-do check if this can be obtained using the fractal kinetics , see for example Bakalis and Zerbetto, “Adsorption Kinetics.”


# Gamma function
- Aspridou, Zafiro, and Konstantinos P. Koutsoumanis. “Individual Cell Heterogeneity as Variability Source in Population Dynamics of Microbial Inactivation.” _Food Microbiology_ 45 (February 2015): 216–21. [https://doi.org/10.1016/j.fm.2014.04.008](https://doi.org/10.1016/j.fm.2014.04.008).
## more advanced

-  [Comparison of unstructured kinetic bacterial growth models.](https://www.sciencedirect.com/science/article/pii/S1026918520300391) !
# To read #to-do
[Survival_function](https://en.wikipedia.org/wiki/Survival_function)