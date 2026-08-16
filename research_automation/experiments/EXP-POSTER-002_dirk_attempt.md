# EXP-POSTER-002 — DIRK Attempt for American Option Pricing

## Purpose

Poster-update experiment exploring a higher-order / alternative time-integration direction beyond the original Crank–Nicolson + PSOR baseline.

## Research question

Can a DIRK-based method improve the accuracy–efficiency trade-off relative to the strengthened classical benchmark for American option pricing?

## Benchmark hierarchy

1. CN–PSOR: original baseline.
2. CN–Policy Iteration: strengthened LCP benchmark.
3. DIRK: experimental extension to be evaluated against the strongest classical benchmark.

## Experiment status

DIRK has been included as a poster-update experimental direction and should be evaluated under the same financial problem and comparable numerical settings.

## Required evaluation dimensions

- option price / pricing error
- runtime
- convergence behavior
- grid sensitivity
- time-step sensitivity
- stability
- comparison against CN–Policy Iteration

## Current interpretation

The value of the DIRK experiment is not merely adding another algorithm. It tests whether changing the time-integration strategy can produce a meaningful improvement over the classical CN-based benchmark.

No unsupported quantitative superiority claim is recorded here. A claim such as “DIRK is more accurate” or “DIRK is faster” should only be promoted to the poster after the corresponding local result tables are verified.

## Next experiments

1. Run controlled grid/time-step refinement.
2. Compare error at matched computational budgets.
3. Record runtime and convergence metrics.
4. Test sensitivity across volatility, interest rate, maturity, and moneyness.
5. Decide whether DIRK should appear as a final poster result, a promising extension, or a negative/neutral experiment.

## Poster relevance

DIRK represents the numerical-method extension beyond the original poster and should be presented only with benchmark-grounded evidence.