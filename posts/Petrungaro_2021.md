# Can we predict evolution of AMR using systems biology?

### Paper

[Petrungaro, Gabriela, Yuval Mulla, and Tobias Bollenbach. “Antibiotic Resistance: Insights from Evolution Experiments and Mathematical Modeling.” *Current Opinion in Systems Biology* 28 (December 2021): 100365](https://doi.org/10.1016/j.coisb.2021.100365).

### What is being predicted

The review explains efforts to predict the evolution of antibiotic resistance by understanding how bacterial populations acquire, establish, and fix beneficial resistance mutations. It focuses on predicting:

- Which resistance mutations will appear and dominate in evolving populations, based on fitness effects, lineage tracking, and mutation–environment interactions. 
- How initial genotype (“genetic background”) shapes resistance evolvability, including epistatic constraints that make some mutational pathways accessible or inaccessible. 
- How resistance trajectories depend on environmental conditions, such as nutrient availability and antibiotic concentration, through quantitative physiological models (e.g., growth‑law–based predictions for translation‑targeting antibiotics). 
- How different evolution protocols influence predicted outcomes, since selection pressure scheduling can drastically alter resistance gains

Overall, prediction targets both short‑term dynamics (mutation establishment and lineage competition) and long‑term adaptive outcomes (dominant mechanisms of resistance under given conditions).

For a similar review, but newer see [Charlebois_2023](Charlebois_2023.md)

### How

The prediction approach is systems‑biology‑driven, combining high‑throughput experimentation with mathematical modeling:

- Massively parallel evolution experiments track large numbers of lineages via chromosomal barcoding and next‑generation sequencing, enabling quantitative inference of fitness distributions and stochastic population dynamics. 
- Controlled experimental systems (e.g., morbidostats, automated evolution platforms) regulate population size and real‑time selection pressure to reveal evolutionary trajectories under reproducible conditions. [Pedreira_2026](Pedreira_2026)
- Mathematical and stochastic models integrate mutation rates, phenotypic delay, demographic noise, and competition to predict establishment probabilities and patterns of fixation.
- Quantitative cell‑physiology models (growth laws linking ribosomes, growth rate, and drug effects) allow prediction of environment‑dependent fitness trade-offs and resistance mechanisms.
- Genome‑wide perturbation screens identify genes that modulate evolvability; this feeds into predictive frameworks by mapping how genetic architecture constrains mutational pathways. 

Together, these layers create an integrated modelling–experiment pipeline capable of forecasting resistance development under specific genetic and environmental contexts.

### Limitations/open problems

Overall, despite major advances, the field is still far from robust clinical‑grade predictions due to complexity, stochasticity, and environmental context dependence.

- Focused on antibiotics, not discussing non-antibiotics antimicrobials

<!--
02/02/2026 I have read mainly the first part of the paper, I like it a lot the discussion about reproducibility and ability to predict the final distribution 
-->

<!--- 03/02/2026--
