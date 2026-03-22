# credit-risk-model-validation-and-explainability
Credit risk PD modeling on 25,000+ borrower records | Logistic Regression · Random Forest · XGBoost | ROC-AUC · KS Statistic · Calibration | SHAP Explainability | Risk Banding | Power BI

# 🏦 Credit Risk Model Validation & Explainability

Built a **Probability of Default (PD)** model on 25,000+ borrower records to identify credit risk drivers and support loan approval decisions.

---

## Dataset
- 25,000+ borrower records
- 20 features — loan details, demographics, credit history
- Target: Risk / No Risk → 1 / 0

## Tech Stack
Python · pandas · scikit-learn · XGBoost · SHAP · matplotlib · seaborn · Power BI

## What I Did
- Trained and compared Logistic Regression, Random Forest, and XGBoost
- Evaluated models using ROC-AUC, Gini, KS Statistic, and Calibration
- Validated performance at segment level (Job, Housing, Credit History)
- Analyzed time-based default rate trends
- Used SHAP to identify key risk drivers and explain individual predictions
- Translated predicted PD into risk bands for approval prioritization
- Exported results to Power BI for dashboard reporting

## Results
| Model | ROC-AUC | KS Statistic |
|---|---|---|
| Logistic Regression | ~0.75 | ~0.38 |
| Random Forest | ~0.78 | ~0.42 |
| XGBoost | ~0.80 | ~0.45 |

XGBoost performed best across all metrics. CheckingStatus and CreditHistory were the strongest default predictors per SHAP.

---

## Screenshots

![Model Performance](screenshots/01_model_performance_table.png)
![ROC Curves](screenshots/02_roc_curves.png)
![KS Plot](screenshots/03_ks_plot.png)
![Monthly Trend](screenshots/04_monthly_trend.png)
![SHAP Beeswarm](screenshots/05_shap_beeswarm.png)
![SHAP Waterfall](screenshots/06_shap_waterfall.png)
![Risk Banding](screenshots/07_risk_banding.png)
