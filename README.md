# Healthcare Insurance Charge Prediction

A machine learning project predicting individual healthcare insurance charges based on demographic and health-related features — demonstrating end-to-end regression modelling with interpretability.

---

## Problem Statement

Healthcare insurers price policies based on risk factors. This project builds a regression model to predict annual insurance charges from customer attributes, then analyses which factors drive cost most significantly. The goal is both predictive accuracy and business interpretability.

---

## Dataset Features

| Feature | Type | Description |
|---------|------|-------------|
| age | Numeric | Customer age in years |
| sex | Categorical | Male / Female |
| bmi | Numeric | Body mass index |
| children | Numeric | Number of dependants |
| smoker | Binary | Smoker status (yes/no) |
| region | Categorical | US geographic region |
| charges | Numeric | **Target** — annual insurance cost (USD) |

---

## Approach

```
Raw Dataset
     │
     ▼
Exploratory Data Analysis
(distributions, outliers, correlations, smoker vs non-smoker split)
     │
     ▼
Preprocessing
(encoding categorical variables, scaling numerics, outlier handling)
     │
     ▼
Model Training and Comparison
(Linear Regression, Ridge, Random Forest, Gradient Boosting)
     │
     ▼
Evaluation
(RMSE, MAE, R² score, residual analysis)
     │
     ▼
Feature Importance Analysis
(which variables drive cost predictions most strongly)
```

---

## Key Findings

- Smoking status is by far the strongest predictor of insurance charges
- BMI interacts significantly with smoking status (high-BMI smokers cluster in the highest cost band)
- Age has a linear positive relationship with charges
- Full results, plots, and model comparison table available in the notebook

---

## Model Comparison

| Model | RMSE | R² | Notes |
|-------|------|----|-------|
| Linear Regression | — | — | See notebook |
| Ridge Regression | — | — | See notebook |
| Random Forest | — | — | See notebook |
| Gradient Boosting | — | — | Best performer |

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat&logo=pandas&logoColor=white)

- Python, pandas, NumPy
- scikit-learn (regression models, preprocessing, evaluation)
- matplotlib, seaborn (visualisation and residual plots)
- Jupyter Notebook

---

## Project Structure

```
Healthcare-Insurance-Prediction/
│
├── notebooks/
│   ├── 01_eda.ipynb                   # Exploratory data analysis
│   ├── 02_preprocessing.ipynb         # Encoding, scaling, outlier handling
│   └── 03_modelling_evaluation.ipynb  # Model training, comparison, feature importance
│
├── data/
│   └── insurance.csv                  # Dataset (source: Kaggle)
│
├── requirements.txt
└── README.md
```

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/zainhammagi12/Healthcare-Insurance-Prediction

# Run notebooks in order
jupyter notebook notebooks/
```

---

## Author

**Zain Hammagi** — [linkedin.com/in/zain-hammagi](https://linkedin.com/in/zain-hammagi) · [zainhammagi.github.io](https://zainhammagi.github.io)
