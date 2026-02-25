# Credit Risk Modelling — Australian P2P Lending Platform

> Loan default prediction for an Australian bank that acquired a peer-to-peer lending platform.  
> Built using GLMs, mixed-effects modelling, and ROC/AUC evaluation — with an executive-level report delivered to management.

---

## Business Problem

An Australian bank acquired a peer-to-peer lending platform and needed to assess the credit risk of its existing loan portfolio. The key questions were:

- Is the platform's existing risk model adequate?
- What borrower and regional factors drive loan default?
- How should the bank adjust its lending policy going forward?

This project builds and validates a suite of predictive models to answer those questions, and translates the results into management-ready recommendations.

---

## What I Built

| Component | Description |
|---|---|
| Baseline GLM | Logistic (logit) and probit regression models for default prediction |
| Benchmark Comparison | Evaluated new models against the platform's existing production model |
| Mixed-Effects Model | Extended baseline to capture geographic and temporal variation in credit risk |
| Model Evaluation | ROC curves, AUC, Gini scores with confidence intervals |
| Executive Report | "Summary on a Page" translating statistical outputs into policy-ready insights |

---

## Key Results

- Achieved AUC improvement over the existing benchmark model
- Identified key regional variation in default rates using mixed-effects modelling
- Delivered a fully reproducible RMarkdown report with executive summary
- Clearly distinguished statistically significant drivers of credit risk for lending policy decisions

---

## Tech Stack

| Tool | Purpose |
|---|---|
| R / RMarkdown | Statistical modelling, reproducible reporting |
| Python | Data preprocessing, exploratory analysis |
| GLM (logit/probit) | Default prediction models |
| lme4 (mixed-effects) | Geographic/temporal variation modelling |
| ggplot2 | Data visualisation |
| ROC / AUC / Gini | Model performance evaluation |

---

## Repo Structure

```
credit-risk-modelling-australia/
│
├── data/
│   └── README.md               # Data description (raw data not included for privacy)
│
├── notebooks/
│   └── 01_exploratory_analysis.ipynb
│   └── 02_data_preprocessing.ipynb
│
├── models/
│   └── credit_risk_model.Rmd   # Main modelling file (R)
│   └── mixed_effects_model.R   # Mixed-effects extension
│
├── report/
│   └── executive_summary.pdf   # Summary on a Page for management
│   └── full_report.pdf         # Full reproducible report
│
├── outputs/
│   └── roc_curve.png
│   └── model_comparison.png
│
└── README.md
```

---

## Business Relevance

This project mirrors a real workflow in banking and financial services:

- Risk analysts use GLMs daily for credit scoring
- Mixed-effects models are standard for capturing portfolio-level variation
- Executive summaries are the primary deliverable in BA and data science roles

**Target roles this project supports:** Data Scientist · Business Analyst · Risk Analyst · Credit Analyst · Data Analyst (Finance)

---

## How to Run

### R Models
```r
# Install dependencies
install.packages(c("lme4", "ggplot2", "pROC", "knitr"))

# Knit the full report
rmarkdown::render("models/credit_risk_model.Rmd")
```

### Python Notebooks
```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Launch notebooks
jupyter notebook notebooks/
```

---

## About This Project

Completed as part of the **MXN600 Advanced Statistical Analysis** unit at Queensland University of Technology (QUT).  
The dataset represents real-world loan portfolio data from an Australian peer-to-peer lending platform.

---

*Part of my data science portfolio — [github.com/Nima-Ghamari](https://github.com/Nima-Ghamari)*
