# Solution guide — A/B Testing and Experiment Design

These are **worked approaches**, not universal numeric answers; estimates depend on data and assumptions.

1. Treatment is the exposure or intervention column; outcome is the measured response.
2. Specify ATE, ATT, ITT, LATE, or local cutoff effect as appropriate; do not substitute one for another.
3. Candidate confounders include baseline spending, age and loyalty in observational marketing data.
4. Identification depends on design: randomization; conditional exchangeability and overlap; parallel trends; IV exclusion; or RDD continuity.
5. `df.info()` and `df.head()` summarize schema.
6. `df.isna().sum()` reports missingness.
7. `df.groupby('treated').size()` or group counts for the relevant dataset.
8. `df.groupby('treated')[covariates].mean()` assesses crude balance; standardized mean differences are preferable.
9. `df.groupby('treated').outcome.mean().diff().iloc[-1]` after using the correct outcome column.
10. Run `Examples.ipynb`, report estimate, population and units; note assumptions.
11. Unmeasured confounding, noncompliance, time-varying shocks, or threshold manipulation can bias estimates.
12. Use pre-treatment outcomes or unaffected negative-control outcomes where feasible.
13. Vary model specification, matching caliper, bandwidth or pre-trend windows depending on design.
14. Provide confidence intervals, design-based standard errors or bootstrap where appropriate.
15. Frame conclusions conditional on the identifying assumptions and sample generalizability.

**Additional exercise:** Re-run using a different synthetic random seed and explain why estimates change.
