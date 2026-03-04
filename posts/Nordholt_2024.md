# Can we predict  persisters presence for *E. coli* exposed to six disinfectants from time-kill data?

### Paper

[Nordholt, Niclas, Lydia-Yasmin Sobisch, Annett Gödt, Dominique Lewerenz, and Frank Schreiber. “Heterogeneous Survival upon Disinfection Underlies Evolution of Increased Tolerance.” _Microbiology Spectrum_ 12, no. 12 (2024): e03276-22. ](https://doi.org/10.1128/spectrum.03276-22).

### What is being predicted
The work focused on models and indices to estimate the persisters behaviour when disinfection with six different compounds (hydrogen peroxide, glutaraldehyde, chlorhexidine, benzalkonium chloride, dicecyldimethylammonium chloride and isopropanol) and using only time-kill curves as experimental data.

### How
It uses two relevant tools
- A mathematical model with two strains dynamics with different killing kinetics (susceptible and persistant cells) following the weibull distribution (although presented in dynamic form). See [models_microbial_dynamics](../topics/models_microbial_dynamics.md) for details
- The evolvability score:  that considers the number of replicate populations, which survive the evolution experiment, the time needed to adapt, and the extent of adaptation in terms of increased survival. Evolvability scores were calculated for each replicate population. For this, the survival fraction at each transfer was normalized by the initial survival fraction
Model calibration using hybrid (DE + local), and comparing removing some of the model parameterse (to determine if there are persistant cells) using the Akaike

### Limitations/open problems
- Using Weibull distribution, instead of common dynamics derived from kinetics, therefore problems using antimicrobial dynamics.

<!--
10/02/2026 I
-->
