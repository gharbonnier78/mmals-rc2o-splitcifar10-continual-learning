# Reproducibility note

Run target:

- `RUN_MODE = robust`
- `DATASET_NAME = SplitCIFAR10`
- seeds: `[0, 1, 2, 3, 4]`
- tasks: five disjoint pairs `(0,1), (2,3), (4,5), (6,7), (8,9)`
- epochs per task: 8
- memory per class/task: 256
- input representation: `small_cnn_feature`
- feature dimension: 256
- A1 backbone reuse: enabled

Baseline hardening uses validation-memory selection only. Final-test results are not used to select baseline hyperparameters or RC2O policy candidates.

The package includes selected raw CSVs under `data/robust/raw_selected/`; the original full Colab package can be kept outside GitHub if size is a concern.
