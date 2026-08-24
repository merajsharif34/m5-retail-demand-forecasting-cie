# Reproducibility guide

## 1. Environment

The final notebook metadata identifies a Python 3 environment and was prepared for a Kaggle-style execution environment.

Install the packages listed in `requirements.txt` if you are running outside Kaggle.

## 2. Data

Do not commit raw M5 or DataCo data. Follow `data/README.md`.

## 3. Notebook

Run:

`notebooks/M5_CIE_Thesis_and_Journal_FINAL_Reproducible.ipynb`

The notebook contains the original RQ1–RQ7 analysis flow plus the final publication/export layer.

## 4. Expected research structure

- RQ1: feature configuration
- RQ2: engineered feature contribution
- RQ3: core model comparison
- RQ4: financial implications
- RQ5: service-level safety stock
- RQ6: uncertainty and safety-stock implications
- RQ7: demand-regime robustness
- External validation: DataCo SMART SUPPLY CHAIN

## 5. Manuscript

The submission source is `manuscript/main.tex`.

Compile it with the Elsevier `elsarticle` class and the bibliography in `manuscript/Bibliography.bib`.

## 6. Important reproducibility principle

Do not silently change reported numerical findings in the manuscript. If a rerun produces a discrepancy, investigate the data, environment, and execution path before updating the paper.
