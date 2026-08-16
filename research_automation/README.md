# Research Automation Framework

This directory is the reproducible experiment-control layer for the SURF2026 research project.

## Research loop

```text
Hypothesis
   ↓
Experiment design
   ↓
Implementation
   ↓
Benchmark / validation
   ↓
Metrics + figures
   ↓
Interpretation
   ↓
Self-critique
   ↓
Next experiment
   ↓
Git commit
```

## Rules

1. **Raw data is immutable.** Never modify, overwrite, rename, or delete files under `data/raw/`.
2. **No secrets.** Never commit API keys, credentials, tokens, `.env` files, private keys, or machine-specific secrets.
3. **Reproducibility first.** Every meaningful experiment must record its method, parameters, data version/reference, software environment, metrics, runtime, and random seed where applicable.
4. **Failed experiments are research evidence.** Do not silently delete failed runs. Record why they failed and what was learned.
5. **Comparisons must be fair.** Preserve the same problem definition, dataset, tolerance, grid/time resolution, and evaluation protocol unless the experiment explicitly studies those factors.
6. **Never overwrite a previous result.** Create a new experiment ID for materially different runs.
7. **Commit meaningful milestones.** Use descriptive commit messages and keep the repository history as the research timeline.

## Directory conventions

- `experiments/`: one directory per experiment/run.
- `results/`: generated metrics, tables, and figures that are useful for research review.
- `reports/`: human-readable research logs and summaries.
- `improvement/`: hypotheses, failure analysis, and proposed next experiments.
- `prompts/`: prompts/instructions used to drive automated research workflows.

## Experiment IDs

Use monotonically increasing IDs such as `EXP-001`, `EXP-002`, etc. Do not reuse an ID.

## Required experiment record

Each experiment should capture:

- research question / hypothesis
- baseline and benchmark
- method
- mathematical or algorithmic changes
- parameters
- implementation path
- data/reference path
- execution command
- seed
- runtime
- accuracy/error metrics
- convergence information where applicable
- comparison with the current best method
- interpretation
- limitations
- self-critique
- next proposed experiment

The goal is not merely to automate code execution, but to maintain an auditable and reproducible computational research process.