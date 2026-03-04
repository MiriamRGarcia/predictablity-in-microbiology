# Can we predict heterogeneity in cell inactivation?
**Paper**

[Aspridou, Zafeiro, Athanasios Balomenos, Panagiotis Tsakanikas, Elias Manolakos, and Konstantinos Koutsoumanis. “Heterogeneity of Single Cell Inactivation: Assessment of the Individual Cell Time to Death and Implications in Population Behavior.” _Food Microbiology_ 80 (June 2019): 85–92.](https://doi.org/10.1016/j.fm.2018.12.011).

**What is being predicted**
- Instead of using the common [Weibull distribution](https://en.wikipedia.org/wiki/Weibull_distribution "Weibull distribution"),
- The log-logistic model assumes that the inactivation times $t_i$ follow a Log-Logistic distribution. Let $N(t_i)$ denote the number of surviving individuals at time $t_i$ Then the survival function can be written as $$ N(t_i) = N_0 \, \mathrm{Rank}(t_i), $$ where $N_0$ is the initial population size and $\mathrm{Rank}(t_i)$ is the rank-based estimate of the survival probability associated with time $t_i$. We assume $$t_i \sim \mathrm{LogLogistic}(\alpha, \beta), \quad i = 1,2,3,\ldots, N, $$ where $\alpha$ is the scale parameter and $\beta$ is the shape parameter. In this case, $\alpha = 45.957, \quad \beta = 2.8583.$ The probability density function (pdf) of a Log-Logistic distribution is $$f(t \mid \alpha,\beta) = \frac{\beta}{\alpha} \left( \frac{t}{\alpha} \right)^{\beta - 1} \left[ 1 + \left( \frac{t}{\alpha} \right)^{\beta} \right]^{-2}, $$ for \(t > 0\). The corresponding survival function is \[ S(t) = \frac{1}{1 + \left( \frac{t}{\alpha} \right)^{\beta}}, \] which provides the expected proportion of individuals surviving beyond time \(t\). Thus, \[ N(t) = N_0 \, S(t) = \frac{N_0}{1 + \left( \frac{t}{\alpha} \right)^{\beta}}. \]

**How**
- Using different distributions and @Risk software



**Limitations/open problems**
 
- Using distributions instead of dynamics

# Further reading

- Using the Gamma function instead of the LogLogistic: Aspridou, Zafiro, and Konstantinos P. Koutsoumanis. “Individual Cell Heterogeneity as Variability Source in Population Dynamics of Microbial Inactivation.” _Food Microbiology_ 45 (February 2015): 216–21. [https://doi.org/10.1016/j.fm.2014.04.008](https://doi.org/10.1016/j.fm.2014.04.008). 