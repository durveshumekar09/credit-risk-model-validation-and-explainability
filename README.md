# 🏦 Credit Risk Model Validation & Explainability

Probability of Default (PD) modeling on 25,000+ borrower records using machine learning. Built to identify key risk drivers, validate model performance, and support loan approval decisions.

---

## Tech Stack
`Python` `pandas` `scikit-learn` `XGBoost` `SHAP` `matplotlib` `seaborn` `Power BI`

---

## Dataset
- 25,000+ borrower records
- 20 features — loan details, credit history, demographics
- Target: `Risk` / `No Risk` → `1` / `0`

---

## Approach
- Trained **Logistic Regression, Random Forest, XGBoost** and compared performance
- Evaluated using **ROC-AUC, Gini, KS Statistic, Brier Score, Calibration**
- Validated model across segments — Job type, Housing, Credit History
- Monitored **monthly default rate trends** to detect portfolio drift
- Applied **SHAP** for global and individual prediction explainability
- Bucketed predicted PD into **4 risk bands** for approval prioritization
- Exported outputs as CSVs for **Power BI** dashboard reporting

---

## Model Performance

| Model | ROC-AUC | Gini | KS Statistic | Brier Score |
|---|---|---|---|---|
| Logistic Regression | 0.8660 | 0.7320 | 0.5685 | 0.1486 |
| Random Forest | 0.9448 | 0.8896 | 0.7452 | 0.1062 |
| **XGBoost** | **0.9856** | **0.9712** | **0.9076** | **0.0436** |

> XGBoost outperformed across all metrics with AUC of 0.9856 and KS Statistic of 0.9076. `CheckingStatus` and `CreditHistory` were the strongest default predictors per SHAP.

---

## Screenshots

Please refer the screenshots in repository
