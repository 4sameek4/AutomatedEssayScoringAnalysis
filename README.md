# Machine Learning for Automated Essay Scoring : Classification or Regression
## 📌 Project Overview

This project presents a lightweight and interpretable Automated Essay Scoring (AES) system designed for low-resource environments. Using a statistically justified dataset and a carefully optimized feature set, the system demonstrates that simple regression-based models can approximate human essay grading with near-perfect agreement.

Despite using only 141 essays and 53 optimized features, the proposed approach achieves a Quadratic Weighted Kappa (QWK) score of 0.9595, validating the effectiveness of regression models over traditional classification approaches for essay scoring.

## 📊 Dataset & Statistical Design

Total essays used: 141

Statistically required minimum: 113 essays

Study design: Sample size exceeded the calculated minimum to ensure statistical reliability

The dataset was intentionally kept small to simulate real-world low-resource scenarios, where large labeled corpora are often unavailable.

## 🔎 Feature Engineering & Selection

Initial feature space: 1,221 features

Feature reduction method: Univariate Feature Selection

Final feature set: 53 optimized features, including:

Top 50 word-count features

Unique word count

Stopword count

This aggressive feature reduction improved model interpretability, reduced overfitting, and preserved predictive performance.

## 🤖 Models & Methodology

The task was modeled primarily as a regression problem, rather than classification, to better capture the ordinal nature of essay scores.

**🔹 Gradient Boosting Regressor (Best Model)**

Quadratic Weighted Kappa (QWK): 0.9595

RMSE: 0.9264

**🔹 Baseline / Comparison Models**

**K-Nearest Neighbors (Classifier):**

QWK: 0.6266

Regression models consistently outperformed classification-based approaches, confirming that essay scoring is best treated as a regression task.

## 📈 Evaluation Metrics

Quadratic Weighted Kappa (QWK) – primary metric for human-level agreement

Root Mean Squared Error (RMSE) – error magnitude assessment

QWK was selected due to its widespread use in AES research and its sensitivity to ordinal misclassification.

## ✅ Key Findings

Achieved near-human agreement with QWK = 0.9595 using a lightweight model

Demonstrated that simple, interpretable regression models can outperform complex classifiers

Validated that 53 carefully chosen features are sufficient for accurate essay scoring

Proved feasibility of AES in low-resource settings without deep learning or large datasets

## 🌍 Impact & Applications

Educational technology in low-resource regions

Rapid essay evaluation for large-scale assessments

Interpretable AES systems for academic and institutional use

## 🔮 Future Work

Expand to multi-prompt and cross-domain datasets

Explore hybrid linguistic and semantic features

Deploy as a real-time AES evaluation tool
