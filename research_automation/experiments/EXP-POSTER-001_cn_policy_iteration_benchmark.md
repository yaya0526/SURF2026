# EXP-POSTER-001 — CN Policy Iteration Benchmark

## Purpose

Poster-update experiment conducted to strengthen the numerical benchmark for the American option LCP solver.

## Research question

Can Crank–Nicolson combined with Policy Iteration provide a stronger and faster benchmark than the existing Crank–Nicolson + PSOR implementation for the same LCP?

## Baseline

- Existing benchmark: CN–PSOR
- Problem: American option pricing formulated as a Linear Complementarity Problem (LCP)
- Comparison principle: keep the same option parameters, spatial grid, time grid, stopping criterion/tolerance, and evaluation protocol whenever possible.

## Experiment

Implemented and tested CN–Policy Iteration on the same LCP setting used for CN–PSOR.

## Observed result

- CN–Policy Iteration successfully solves the same LCP.
- CN–Policy Iteration was observed to be faster than CN–PSOR in the completed poster-update tests.
- This provides a stronger computational benchmark candidate because the comparison is made on the same underlying LCP rather than changing the pricing problem.

## Interpretation

The result suggests that PSOR should no longer be treated as the only numerical benchmark. Policy Iteration gives a useful complementary reference for the LCP solve and improves the computational baseline used for subsequent methods.

## Limitations / items to preserve from raw experimental outputs

The exact runtime, iteration count, grid/time-step configuration, and numerical error should be copied from the final local experiment outputs before publication. This record intentionally does not invent quantitative values that are not present in the current research log.

## Next step

Compare DIRK against the strengthened CN–Policy Iteration benchmark using accuracy/error, runtime, convergence behavior, and grid/time-step refinement.

## Poster relevance

This experiment supports replacing or supplementing CN–PSOR with CN–Policy Iteration as the strengthened benchmark in the updated poster.