# Research Improvement Queue

This file is the controlled queue for subsequent experiments. New ideas should be justified by evidence from completed experiments rather than added arbitrarily.

## Priority queue

### P0 — Establish controlled baseline

- Register the existing benchmark implementation as an explicit experiment.
- Record solver parameters, grid sizes, tolerances, runtime and convergence information.
- Preserve the exact configuration so later methods can be compared fairly.

### P0 — Benchmark strengthening

- Compare CN-PSOR against CN-Policy Iteration on identical LCP instances.
- Measure runtime, iterations, price error and convergence behavior.
- Determine whether Policy Iteration is a stronger computational benchmark.

### P1 — Accuracy / efficiency comparison

- Evaluate DIRK against the strongest CN benchmark.
- Separate temporal discretization error from spatial discretization error.
- Report error-versus-runtime rather than accuracy alone.

### P1 — Robustness

- Vary grid resolution and time step.
- Test parameter sensitivity across volatility, interest rate, maturity and moneyness.
- Check whether conclusions remain stable under different numerical settings.

### P2 — Method improvement

- Explore adaptive discretization or other justified numerical improvements only after the benchmark is stable.
- Compare against the current best method using the same evaluation protocol.

## Rule for adding experiments

Every new experiment must answer a concrete research question. If a method does not improve accuracy, efficiency, stability, or scientific understanding, document the negative result and do not continue blindly.
