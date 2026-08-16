# Self-Critique — EXP-XXX

## A. Validity checks

- Was the implementation independently sanity-checked?
- Were boundary and initial conditions correct?
- Were convergence criteria applied consistently?
- Was the benchmark sufficiently accurate for the claim being made?

## B. Fairness checks

- Same financial parameters?
- Same grid/time resolution where appropriate?
- Same tolerance?
- Same stopping criterion?
- Same hardware/environment where runtime is compared?

## C. Numerical checks

- Does error decrease under refinement?
- Is the observed convergence rate plausible?
- Are there oscillations, instability, or solver failures?
- Are results sensitive to tolerance or initialization?

## D. Statistical / reporting checks

- Are enough parameter regimes tested?
- Is one favorable case driving the conclusion?
- Are both accuracy and runtime considered?
- Are negative results retained?

## E. Alternative explanations

List the strongest reasons why the observed improvement might not be caused by the proposed method.

## F. Next test

Design the smallest experiment that can distinguish between the leading explanations.
