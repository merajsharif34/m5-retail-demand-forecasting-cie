# A Data-Driven Framework for Retail Demand Forecasting and Financial Impact Evaluation Using the M5 Benchmark Dataset

Reproducibility repository for the manuscript prepared for *Computers & Industrial Engineering* (Elsevier).

## Repository purpose

This repository preserves the journal-study source materials needed to inspect the analysis, manuscript, supplementary material, and submission assets.

**Source of truth for empirical results:** the final journal notebook in `notebooks/`. The thesis is not used as the numerical authority for the journal manuscript. If an older document and the final journal notebook differ, the journal notebook is the reference for the journal results.

## Study at a glance

- **Primary dataset:** M5 Forecasting Accuracy competition dataset
- **Series selection:** 500 highest-volume item-store series using training-period demand only
- **Evaluation:** chronological 28-day hold-out
- **Test observations:** 14,000
- **Core models:** Linear Regression, Random Forest, XGBoost
- **Supporting analyses:** LightGBM and ARIMA
- **Research questions:** RQ1-RQ7
- **External robustness check:** DataCo SMART SUPPLY CHAIN dataset

## Repository structure

```text
.
├── README.md
├── CITATION.cff
├── .gitignore
├── requirements.txt
├── notebooks/
│   └── M5_CIE_Thesis_and_Journal_FINAL_Reproducible.ipynb
├── manuscript/
│   ├── main.tex
│   ├── Bibliography.bib
│   └── supplementary/
│       ├── Supplementary_Material.tex
│       └── Figures/
├── figures/
│   └── README.md
├── submission/
│   ├── CIE_Journal_Submit_Ready.pdf
│   ├── Supplementary_Material.pdf
│   ├── graphical_abstract.pdf
│   ├── Highlights.txt
│   └── README.md
├── data/
│   └── README.md
└── docs/
    ├── REPOSITORY_STATUS.txt
    └── REPRODUCIBILITY.md
```

## Reproducibility

The notebook was prepared for a Kaggle-style execution environment and expects the original M5 competition files under the Kaggle input tree. DataCo is used only when the optional external-validation data are available.

Raw M5/DataCo datasets are intentionally not committed. Follow `data/README.md` for data-access instructions.

The notebook contains the RQ1-RQ7 analysis and the publication/export layer. The manuscript source is `manuscript/main.tex`; the supplementary source and supplementary figure PDFs are under `manuscript/supplementary/`.

## Publication assets

`submission/` contains the manuscript PDF, supplementary PDF, graphical abstract, and highlights used for the submission package. Editable manuscript and supplementary sources remain under `manuscript/`.

The `figures/` directory is reserved for principal manuscript figure assets. Supplementary figure PDFs are preserved under `manuscript/supplementary/Figures/`.

## Integrity and versioning

Do not silently change reported numerical findings. If a clean rerun produces a discrepancy, investigate the data, environment, execution path, and source version before changing the manuscript.

Generated runtime artifacts, credentials, raw datasets, and local environments are excluded by `.gitignore`.

## Citation

Please cite the repository and associated manuscript using `CITATION.cff`.

## Authors

- Mohamed Meraj Mansur Sharif
- Raja Hashim Ali
- Talha Ali Khan

Target journal: *Computers & Industrial Engineering* (Elsevier).
