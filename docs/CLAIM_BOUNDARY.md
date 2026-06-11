# Claim boundary

## Supported

- MMALS/RC2O is evaluated in a SplitCIFAR10 continual-learning protocol.
- The visual representation is a supervised A1 SmallCNN perceptual host trained and sanity-checked before CL, then frozen.
- The downstream MMALS/RC2O stack performs continual learning over the frozen 256-dimensional features.
- The robust 5-seed run shows selected RC2O outperforming the best validation-selected replay baseline.
- Specialization diagnostics are materialized and aligned to the selected policy candidate.

## Not supported yet

- End-to-end raw-pixel continual representation learning.
- Broad external-dataset robustness beyond SplitCIFAR10.
- CIFAR10 SOTA.
- Positive backward transfer.

## Paper-safe sentence

RC2O-v2.2c evaluates MMALS in a SplitCIFAR10 class-incremental continual-learning protocol over a frozen supervised visual feature representation.
