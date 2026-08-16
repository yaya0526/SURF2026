# Results

Store research outputs that are useful for reproducibility and review.

Recommended structure:

```text
results/
├── metrics/
├── tables/
└── figures/
```

Use experiment IDs in filenames, for example:

- `EXP-004_metrics.csv`
- `EXP-004_convergence.png`
- `EXP-004_runtime_vs_error.csv`

Large raw datasets and temporary artifacts should remain outside the repository according to the project Git policy.
