# 💡 Customer Churn Explainable Prediction

**Exploratory and Explainable AI analysis of energy customer churn**

This project contains an exploratory data analysis and predictive modeling pipeline for energy customer churn. In addition to building a high-performing model, it emphasizes **explainability** and **uncertainty quantification** to support real-world business decision-making.

---

## 🔍 Overview

The analysis investigates drivers of customer churn in the energy sector, focusing on:

- Consumption patterns (total and gas-specific)
- Sales channels
- Price sensitivity
- Contract duration and customer tenure

---

##  Key Findings

- **Overall churn rate**: ~9.7%
- **Top churn predictors**:  
  - Net margin on power subscriptions  
  - Gas and electricity consumption over 12 months  
  - Contract duration
- **Price sensitivity**: Less impactful than expected
- **Sales channels**: Churn varies significantly across channels — potential for strategic optimization

---

##  Predictive Model

A **Random Forest Classifier** was used to predict churn, achieving:

- **Accuracy**: 90.36%  
- **Precision**: 81.82%  
- **Recall**: 4.92%

The model was interpreted using **SHAP values** to ensure transparency in feature contributions.

---

##  Explainability & Uncertainty

### SHAP Interpretability
SHAP (SHapley Additive exPlanations) was used to identify:
- **Top global drivers** of churn
- **Feature interactions** (e.g., gas usage × contract length)
- **Individual predictions** explanation for case-level insight

<insert SHAP summary bar chart and interaction plot screenshots if uploading images>

### Confidence Intervals
Uncertainty was visualized via bootstrapped metrics and prediction confidence levels to support:
- **Better decision-making**
- **Trust in the model's output**

---

## 💼 Business Impact

This project enables:

-  **Early churn detection** for proactive intervention  
-  **Targeted retention campaigns** for high-risk customers  
- **Revenue preservation** by focusing efforts where they matter most  
-  Continuous improvement with explainability built into every update

---

## 🛠 Tools Used

- Python
- Pandas
- Matplotlib, Seaborn
- Scikit-learn
- SHAP

---

## Possible Next Steps

- Integrate early warning system into CRM  
- Run A/B testing for tailored retention strategies  
- Add economic cost-benefit layer to predictions  
- Refine model with new features (e.g., seasonal usage)

---

## 📄 License

This project is open source and available under the MIT License.
