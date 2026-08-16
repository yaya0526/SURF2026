# Scientific Machine Learning and Numerical Methods in Derivative Pricing

This repository records my learning progress and computational research during the SURF project.

## Research topics

- Option Fundamentals
- Risk-Neutral Pricing
- Binomial Tree Methods
- Black-Scholes Model
- Black-Scholes PDE
- Finite Difference Methods
- Crank-Nicolson Scheme
- American Options
- Free Boundary Problems
- Linear Complementarity Problems
- Physics-Informed Neural Networks (PINNs)
- Deep Galerkin Methods (DGM)

## Automated Research Framework

The repository now includes a reproducible research-control layer under `research_automation/`.

It is designed to support the full computational research loop:

```text
Research question
      ↓
Experiment design
      ↓
Implementation
      ↓
Benchmark / validation
      ↓
Metrics + figures
      ↓
Scientific interpretation
      ↓
Self-critique
      ↓
Next experiment
      ↓
Git versioning
```

### Framework components

- `research_automation/prompts/` — prompts and templates for automated research agents
- `research_automation/experiments/` — experiment-by-experiment records
- `research_automation/results/` — reproducible research outputs
- `research_automation/reports/` — chronological research logs
- `research_automation/improvement/` — hypotheses, failure analysis, and next experiments
- `research_automation/research_config.yaml` — project-wide automation rules
- `research_automation/experiment_registry.json` — machine-readable experiment registry

### Core principles

1. Raw data is immutable.
2. Every meaningful experiment is reproducible and uniquely identified.
3. Failed experiments are retained as research evidence.
4. Numerical accuracy, runtime, convergence, and robustness are evaluated separately.
5. Automated self-critique is required before selecting the next experiment.
6. Git history is treated as part of the research record.

The repository also contains weekly reports, lecture materials, handwritten notes, and implementation code.