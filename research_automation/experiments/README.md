# Experiments

Each controlled experiment gets its own immutable record directory.

Recommended structure:

```text
EXP-001_baseline/
├── README.md
├── config.yaml
├── results.csv
├── metrics.json
├── figures/
└── notes.md
```

The directory name must contain a unique experiment ID. Do not overwrite a completed experiment with a later run; create a new experiment ID instead.
