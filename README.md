<!DOCTYPE html>

# Air Quality Index Prediction 🌫️

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=2EC4B6&center=true&vCenter=true&width=620&lines=AQI+Prediction+using+Machine+Learning;Time+Series+%7C+Feature+Engineering;Baseline+%26+Advanced+ML+Models;End-to-End+Jupyter+Notebook+Workflow;MSc+Data+Analytics+Coursework" alt="Typing Animation" />
</div>

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=FFD43B"/>
  <img alt="Jupyter" src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <img alt="Scikit-learn" src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
  <img alt="Pandas" src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img alt="Matplotlib" src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white"/>
</p>

<p align="center">
  <img alt="Type" src="https://img.shields.io/badge/Task-Regression_%2F_Prediction-2EC4B6?style=flat-square"/>
  <img alt="Domain" src="https://img.shields.io/badge/Domain-Environmental_Analytics-CBF3F0?style=flat-square&labelColor=264653"/>
  <img alt="Notebook" src="https://img.shields.io/badge/Reproducible-Jupyter_Notebook-F37626?style=flat-square"/>
  <img alt="License" src="https://img.shields.io/badge/license-MIT-2EC4B6?style=flat-square"/>
</p>

---

## 🌍 Why This Matters

Poor air quality is one of the leading environmental health risks globally — linked to respiratory disease, cardiovascular conditions, and reduced life expectancy. Traditional monitoring relies on dense sensor networks and reactive reporting.

This project takes a **data-driven approach**: using historical air quality and meteorological records to build ML models that can **predict AQI levels before they are measured**, enabling proactive monitoring and informed decision-making.

---

## 🚀 Project Overview

A **full end-to-end machine learning pipeline** for AQI prediction, covering everything from raw data ingestion to evaluated, visualised model outputs — packaged in a single reproducible Jupyter notebook.

<div align="center">

| 📥 **Data Pipeline** | 🔬 **Modelling** | 📊 **Evaluation** |
|---|---|---|
| Raw data ingestion & audit | Baseline models (Linear, KNN) | RMSE · MAE · R² |
| Missing value imputation | Advanced models (RF, XGBoost) | Residual analysis |
| Outlier detection & treatment | Time-series feature engineering | Feature importance plots |
| EDA & correlation analysis | Cross-validation & tuning | Actual vs. predicted plots |

</div>

---

## 🧠 Objectives

- Analyse historical air quality data and identify the key environmental drivers of AQI
- Engineer temporal and meteorological features to capture time-series behaviour
- Build and compare multiple ML models — from simple baselines to ensemble methods
- Evaluate model performance with appropriate regression metrics
- Generate interpretable visualisations to support air quality insights and decision-making

---

## 📁 Repository Structure

```
aqi-prediction-ml/
│
├── 📂 data/
│   ├── raw/
│   │   └── air_quality_raw.csv          # Original dataset (source-linked below)
│   └── processed/
│       └── air_quality_clean.csv        # Cleaned & feature-engineered dataset
│
├── 📂 notebooks/
│   └── AQI_Prediction_Pipeline.ipynb    # Full end-to-end notebook
│
├── 📂 outputs/
│   ├── figures/                         # All EDA & model evaluation plots
│   └── model_comparison.csv             # RMSE / MAE / R² summary table
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation & Running

**1. Clone the repository**
```sh
git clone https://github.com/abinraju23/aqi-prediction-ml.git
cd aqi-prediction-ml
```

**2. Install dependencies**
```sh
pip install -r requirements.txt
```

**3. Launch the notebook**
```sh
jupyter notebook notebooks/AQI_Prediction_Pipeline.ipynb
```

---

## 🔧 Pipeline Walkthrough

### 1 · Data Cleaning & EDA
```
→ Load raw CSV, audit shape and dtypes
→ Handle missing values (mean/median/forward-fill by feature type)
→ Detect and treat outliers (IQR-based capping)
→ Correlation heatmap, distribution plots, seasonal decomposition
```

### 2 · Feature Engineering
```
→ Lag features: AQI(t-1), AQI(t-7), rolling 7-day mean
→ Temporal features: hour, day-of-week, month, season flag
→ Interaction terms: wind × humidity, temp × pollutant concentration
→ Target encoding for categorical meteorological variables
```

### 3 · Model Training & Comparison

| Model | Type | Notes |
|---|---|---|
| Linear Regression | Baseline | Interpretable benchmark |
| K-Nearest Neighbours | Baseline | Distance-based comparison |
| Random Forest | Ensemble | Non-linear, feature importance |
| XGBoost / Gradient Boosting | Ensemble | Primary best-performer |

### 4 · Evaluation Metrics
```
RMSE  — penalises large prediction errors
MAE   — interpretable average absolute error
R²    — proportion of variance explained
```

---

## 📈 Key Results

> *Results from the best-performing model on the held-out test set.*

| Metric | Score |
|---|---|
| RMSE | *(see notebook)* |
| MAE | *(see notebook)* |
| R² | *(see notebook)* |

Feature importance analysis revealed that **[key pollutant / lag feature]** was the strongest predictor of next-period AQI — consistent with domain literature linking PM2.5 persistence to short-term AQI trajectories.

> Update the table above with your actual results once the notebook is run.

---

## 📦 Dependencies

```txt
pandas >= 2.0
numpy >= 1.26
scikit-learn >= 1.4
xgboost >= 2.0
matplotlib >= 3.8
seaborn >= 0.13
jupyter >= 1.0
```

Install all at once:
```sh
pip install -r requirements.txt
```

---

## 👤 Author

**Abin Raju**
MSc Data Analytics — Dublin Business School (September 2025 cohort)

<p>
  <a href="https://www.linkedin.com/in/abinraju2308">
    <img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://github.com/abinraju23">
    <img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
</p>

---

## ⚠️ Disclaimer

This project was developed as part of an academic data analytics coursework. Model outputs are intended for research and educational purposes and should not be used as a substitute for certified air quality monitoring systems.

---

<div align="center">
  <sub>Built with Python · Scikit-learn · XGBoost · Jupyter</sub><br/>
  <sub>© 2026 Abin Raju · MSc Data Analytics · Dublin Business School</sub>
</div>
