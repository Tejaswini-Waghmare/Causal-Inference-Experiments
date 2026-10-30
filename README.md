# Causal Inference and Experiments

Ten educational modules, reproducible Python notebooks, synthetic datasets, exercises and solutions. **Study material, not claims of completed production research.**

## Setup
```bash
python -m venv .venv
# activate your environment
pip install -r requirements.txt
jupyter lab
```
Run notebooks from repository root so relative `data/` paths resolve. In Colab upload the needed CSV file to `/content/`.

## Modules
- [01 Causal Thinking and DAGs](01_Causal_Thinking/README.md)
- [02 Potential Outcomes and Treatment Effects](02_Potential_Outcomes/README.md)
- [03 Randomized Experiments](03_Randomized_Experiments/README.md)
- [04 A/B Testing and Experiment Design](04_AB_Testing/README.md)
- [05 Regression Adjustment](05_Regression_Adjustment/README.md)
- [06 Propensity Scores and Matching](06_Propensity_Scores/README.md)
- [07 Difference-in-Differences](07_Difference_in_Differences/README.md)
- [08 Instrumental Variables](08_Instrumental_Variables/README.md)
- [09 Regression Discontinuity](09_Regression_Discontinuity/README.md)
- [10 End-to-End Causal Case Study](10_End_to_End_Causal_Case_Study/README.md)

## Ethical practice
Use synthetic data only. Do not interpret a regression coefficient as causal without identification assumptions.
