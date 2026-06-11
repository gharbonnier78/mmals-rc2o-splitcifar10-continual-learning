# Scientific demarche

1. **Failure diagnosis.** Early SplitCIFAR runs were weak, making representation failure a plausible confound.
2. **Baseline hardening.** EWC, LwF, replay, PNN and MoE controls were selected by validation traces rather than arbitrary defaults.
3. **Backbone ladder.** A0/A1/A2 representation checks established that the A1 perceptual host provides a usable feature space.
4. **Continual-learning bridge.** MMALS/RC2O was evaluated over frozen A1 features on SplitCIFAR10 disjoint class-incremental tasks.
5. **Audit closure.** Readout collapse, route/context, host ablation, host probe and prototype separation diagnostics were exported and aligned to the selected policy.
6. **Robust run.** The 5-seed robust package confirms the 3-seed evidence trend.
