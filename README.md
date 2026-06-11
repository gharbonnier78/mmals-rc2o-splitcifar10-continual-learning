# MMALS RC2O-v2.2c SplitCIFAR10 Robust Bridge Package

This repository package updates the arXiv/GitHub materials with the **SplitCIFAR10 robust 5-seed addendum**.

<p align="center">
  <a href="./paper/main.pdf">
    <img src="https://img.shields.io/badge/Open-Article-0B5FFF?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Open PDF">
  </a>
  &nbsp;
  <a href="./docs/MMALS_SplitCIFAR10_RC2O_v22c_robust_analysis_report.pdf">
    <img src="https://img.shields.io/badge/Open-Results-111827?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Open PDF">
  </a>
</p>

## Status

**Supported claim:** RC2O-v2.2c evaluates MMALS in a SplitCIFAR10 class-incremental continual-learning protocol over a frozen supervised A1 visual feature representation.

**Not claimed:** end-to-end raw-pixel continual representation learning, CIFAR10 SOTA, or broad external-dataset generality.

## Main robust result

- Selected RC2O: `0.91395 +/- 0.00639`
- Best replay: `0.73860 +/- 0.01559`
- Paired selected-RC2O gain vs replay: `0.17535` with 95% CI `[0.16093, 0.18977]`
- Min-task accuracy: `0.85350`
- Forgetting: `0.02425`
- Min-class recall: `0.84100`
- External-bridge gates passed: `True`

## Structure

- `paper/` - LaTeX source, figures, tables, compiled PDF.
- `data/robust/` - robust addendum CSV/JSON tables plus selected raw robust artifacts.
- `data/evidence/` - earlier 3-seed evidence summaries for continuity.
- `reports/` - robust and evidence analysis PDFs plus notebook PDF export.
- `notebooks/` - v2.2c notebook.
- `docs/` - claim boundary, reproducibility note, scientific demarche, and file manifest.

## Build

```bash
cd paper
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

The precompiled PDF is included as `paper/main.pdf`.

## Release note

This update freezes the package as `RC2O-v2.2c SplitCIFAR10 robust bridge` and should accompany the main MMALS article and the RC2O-specific paper.
