# Customer Churn Explainable Prediction

Exploratory analysis and predictive modeling for energy customer churn, built as part of the BCG Data Science simulation on Forage.

The focus was on understanding what drives churn and making the model's reasoning transparent using SHAP, rather than just optimizing accuracy.

## What the data showed

The dataset covers ~14,000 energy customers. Overall churn rate is about 9.7%. The strongest predictors turned out to be net margin on power subscriptions, gas and electricity consumption over 12 months, and contract duration. Price sensitivity was less impactful than expected, which was the most interesting finding — the simulation brief assumed price was the main driver.

## Model

Random Forest classifier. Accuracy: 90.36%, Precision: 81.82%, Recall: 4.92%. The low recall is worth noting — the model is conservative about predicting churn, which means it misses most actual churners. In a production setting you'd want to tune the threshold or try cost-sensitive learning.

## Explainability

SHAP values were used for both global feature importance and individual prediction explanations. Bootstrapped confidence intervals give a sense of how stable the predictions are. The goal was to make the model's output something a business team could actually act on, not just a score.

## Tools

Python, pandas, matplotlib, seaborn, scikit-learn, SHAP

## Files

- `BCG_Task_2__EDA.ipynb` — exploratory data analysis
- `Churn_Predictive_modeling_.ipynb` — modeling pipeline with SHAP interpretation
