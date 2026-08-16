# Poster Update — Experimental Progress Summary

## Objective

The original poster established a classical American option pricing baseline. The current update aims to strengthen the computational contribution by adding controlled solver comparisons and exploratory numerical improvements rather than simply adding a more complicated model.

## Experimental progression

### Stage 1 — Original benchmark: CN–PSOR

Crank–Nicolson provides the time discretization and PSOR solves the resulting American-option LCP. This remains an important classical reference because it directly handles the early-exercise constraint.

### Stage 2 — Stronger benchmark: CN–Policy Iteration

A Policy Iteration solver was introduced for the same LCP. In the completed poster-update tests, it solved the same problem successfully and was observed to be faster than CN–PSOR. This strengthens the benchmark and prevents subsequent methods from being compared only against a relatively slow iterative baseline.

### Stage 3 — Numerical extension: DIRK

DIRK was introduced as an exploratory time-integration direction. Its role is to test whether a different time discretization can improve the accuracy–efficiency trade-off relative to the strengthened CN benchmark. Quantitative superiority should only be claimed after the final result tables are verified.

## Benchmark philosophy

The updated poster should distinguish three levels clearly:

| Level | Method | Role |
|---|---|---|
| Baseline | CN–PSOR | Original classical benchmark |
| Strong benchmark | CN–Policy Iteration | Faster LCP benchmark observed in current tests |
| Experimental extension | DIRK | Candidate numerical improvement |

## What the poster should demonstrate

The key research contribution should be framed as a reproducible comparison rather than an accumulation of algorithms. For every candidate method, report comparable:

- option value / pricing error
- runtime
- iteration or convergence information where applicable
- spatial-grid resolution
- time-step resolution
- stability / sensitivity

## Current evidence level

### Supported qualitative finding

CN–Policy Iteration is a viable solver for the same American-option LCP and was observed to be faster than the existing CN–PSOR benchmark in the poster-update experiments.

### Pending quantitative verification

Exact runtime ratios, iteration counts, error values, DIRK accuracy claims, and parameter-sensitivity results must be imported from the local experiment outputs before they are treated as final poster evidence.

## Recommended poster narrative

> We first strengthen the classical American-option benchmark by comparing two solvers for the same Crank–Nicolson LCP. Policy Iteration provides a more efficient reference than the original PSOR implementation in our current experiments. We then explore alternative time-integration methods such as DIRK and evaluate whether they improve the accuracy–efficiency trade-off under controlled numerical settings.

## Next automated research cycle

1. Recover and register exact outputs from the poster experiments.
2. Standardize all methods under a common experiment configuration.
3. Run grid and time-step convergence experiments.
4. Compare runtime at matched accuracy and accuracy at matched runtime.
5. Perform parameter sensitivity experiments.
6. Generate publication-ready comparison tables and figures.
7. Run at least three self-critique / refinement cycles before selecting the final poster result.