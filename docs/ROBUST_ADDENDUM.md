# Robust addendum summary

The robust run upgrades the SplitCIFAR10 branch from 3-seed evidence to a 5-seed robust external CL bridge.

| Metric | Value |
|---|---:|
| Selected RC2O final average accuracy | 0.91395 +/- 0.00639 |
| Best replay final average accuracy | 0.73860 +/- 0.01559 |
| Paired gain vs replay | 0.17535 |
| 95% CI for gain | [0.16093, 0.18977] |
| Min-task accuracy | 0.85350 |
| Forgetting | 0.02425 |
| Min-class recall | 0.84100 |
| Oracle gap | 0.00950 |

The row previously named `joint_upper_bound` should be renamed `joint_mlp_control` in article text because RC2O exceeds it; it is not a mathematical upper bound.
