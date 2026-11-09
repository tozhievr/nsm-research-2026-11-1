# Experiment summary — measured results

All values are reported for a **single trained checkpoint** and deliberately selected test expressions. Do not interpret them as out-of-distribution generalization metrics.

## Capacity
| K | Correct / 24 |
|---|---|
| 64 | 14 |
| 65 | 23 |
| 66 | 24 |
| 80 | 24 |

Zeroing additional tail cells at each step reproduces the lower-capacity result in the targeted cases.

## Interventions
Three selected expressions were studied with cell interventions at steps 110–145, cells 63–65. The pair-intervention pilot evaluated 36 pairs: 6 classification flips and 5 nonzero nonlinear interactions.

## Finite differences
45 combinations: 3 expressions, 5 timesteps, 3 cells. At epsilon 0.1, mean absolute directional derivatives by cell were 63: 0.000230; 64: 0.000749; 65: 0.000383. These values are **not** Jacobian norms or global stability guarantees.

## Status
The original PyTorch source, checkpoint and complete JSON logs must still be uploaded to this GitHub repository. Until then, the downloadable research archive is the complete experiment bundle.

## Second generated sample (10 Nov 2026)

Using the same checkpoint and generator protocol but a new seed `20261110`, another 24 targeted expressions yielded K=64: 22/24, K=65: 23/24, K=66: 24/24, K=80: 24/24. This **post-hoc repeat** shows the 64→66 effect size depends strongly on the sample (41.7 vs 8.3 percentage points). The CSV is in `capacity_replication_20261110.csv`.

A reviewed manuscript and full code/checkpoint/JSON bundle were prepared separately for journal submission; the binary items are not yet hosted in this repository.
