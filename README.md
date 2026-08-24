# M5 Retail Demand Forecasting — Computers & Industrial Engineering

Reproducible research repository for:

**A Data-Driven Framework for Retail Demand Forecasting and Financial Impact Evaluation Using the M5 Benchmark Dataset**

This repository contains the final reproducibility notebook and the LaTeX manuscript source prepared for submission to *Computers & Industrial Engineering* (Elsevier).

## Study at a glance

- **Primary dataset:** M5 Forecasting Accuracy competition dataset
- **Series selection:** 500 highest-volume item–store series using training-period demand only
- **Evaluation:** chronological 28-day hold-out
- **Test observations:** 14,000
- **Core models:** Linear Regression, Random Forest, XGBoost
- **Supporting analyses:** LightGBM and ARIMA
- **Research questions:** RQ1–RQ7
- **External robustness check:** DataCo SMART SUPPLY CHAIN dataset

The notebook preserves the thesis-aligned RQ1–RQ7 analyses and includes the publication/export layer used to organize the journal figures and tables.

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
    └── REPRODUCIBILITY.md
```

## Running the analysis

The final notebook was designed around a Kaggle-style environment. It expects the M5 competition files under the Kaggle input tree and optionally uses the DataCo CSV for external validation.

Open:

`notebooks/M5_CIE_Thesis_and_Journal_FINAL_Reproducible.ipynb`

Then run the notebook in the intended environment. The notebook contains the RQ1–RQ7 analyses and publication-output packaging layer.

**Do not upload the raw M5 or DataCo datasets to this repository.** Use the original dataset sources described in `data/README.md`.

## Reproducibility notes

The study design uses training-only series selection and a chronological hold-out. The final publication layer does not introduce a new research design; it packages the existing analyses, figures and tables for manuscript use.

The manuscript source is in `manuscript/main.tex`. The bibliography is provided separately as `manuscript/Bibliography.bib`. The supplementary material — the additional development-stage and diagnostic figures not included as primary manuscript figures — is in `manuscript/supplementary/Supplementary_Material.tex`, with its figures in `manuscript/supplementary/Figures/`; a compiled copy is in `submission/Supplementary_Material.pdf`.

## Research outputs

The final manuscript reports:

- feature-configuration analysis,
- feature-importance analysis,
- core-model comparison,
- financial scenario analysis,
- service-level/safety-stock analysis,
- uncertainty-tier analysis,
- demand-regime robustness analysis,
- DataCo external validation.

The repository intentionally does not contain raw observations, credentials, model checkpoints, or other sensitive/generated runtime artifacts.

## Citation

If you use this repository or the associated research, please cite the paper using the metadata in `CITATION.cff`.

## Authors

- Mohamed Meraj Mansur Sharif
- Raja Hashim Ali
- Talha Ali Khan

Target journal: *Computers & Industrial Engineering* (Elsevier).
