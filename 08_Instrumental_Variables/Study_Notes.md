# 08. Instrumental Variables

## Learning objectives
- Explain relevance, exclusion restriction, wald estimand.
- State the estimand and assumptions before analyzing data.
- Diagnose threats to identification and communicate uncertainty.

## Core ideas
Causal inference asks what would happen to the same unit under different interventions. Because only one outcome is observed for a given unit, causal identification requires a design or explicit assumptions.

### Key terminology
- **Treatment**: intervention or exposure.
- **Outcome**: result of interest.
- **Confounder**: variable affecting treatment and outcome.
- **ATE**: E[Y(1)-Y(0)] for the target population.
- **ATT**: E[Y(1)-Y(0) | treated=1].
- **Consistency**: observed outcomes agree with assigned potential outcome.
- **Positivity**: comparable treated and untreated observations exist.

## This module's method
Relevance, exclusion restriction, Wald estimand. The worked notebook illustrates the method and prints diagnostic information.

## Interpretation checklist
1. Define treatment, outcome, population, time window, and estimand.
2. Describe assignment mechanism and possible confounders.
3. Inspect missingness, balance, and overlap.
4. Compute estimate and uncertainty where supported.
5. Check design-specific assumptions and alternatives.
6. Distinguish correlation from causal identification.

## Cautions
Synthetic data make concepts reproducible but do not prove that assumptions hold in a real setting. Estimates from observational data may be biased by unmeasured confounding; significance is not practical importance.

## Suggested reading
- Hernán & Robins, *Causal Inference: What If* (freely available online).
- Cunningham, *Causal Inference: The Mixtape*.
- Imbens & Rubin, *Causal Inference for Statistics, Social, and Biomedical Sciences*.
