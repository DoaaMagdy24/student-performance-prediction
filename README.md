# 📊 Student Exam Score Prediction with Machine Learning

> Predicting student performance using educational, behavioral, and environmental factors.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-000000?style=for-the-badge&logo=seaborn&logoColor=white)

## 🔍 Project Overview

This project analyzes the **Student Performance Factors** dataset to predict students' final exam scores using various machine learning models. Features include hours studied, parental education, teacher quality, motivation, internet access, and more. The goal is to identify key predictors of academic success.

### 🎯 Objectives
- Clean and preprocess categorical & missing data
- Apply target encoding and label encoding
- Build and compare multiple regression models:
  - Linear Regression
  - Gradient Boosting (with hyperparameter tuning)
  - Polynomial Regression (single & multi-feature)
- Visualize correlations and model performance
- Extract actionable insights for educators and policymakers

## 📂 Dataset

- Source: You can download it from Kaggle [`StudentPerformanceFactors.csv`](https://www.kaggle.com/datasets/laavanya/student-performance-factors)  
- Samples: ~1,000+ students  
- Features: 18+ variables including socio-economic, behavioral, and school-related factors  
- Target: `Exam_Score` (numeric, 0–100)

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas / NumPy | Data manipulation |
| Matplotlib / Seaborn | Visualization |
| Scikit-learn | ML modeling, preprocessing, evaluation |
| Jupyter Notebook | Interactive analysis |

## 📈 Key Results

| Model | R² Score | MSE |
|-------|----------|-----|
| Linear Regression | 0.69 | 4.41 |
| Gradient Boosting | **0.72** | **3.89** |
| Polynomial (single-feature) | 0.19 | 12.12 |
| Polynomial (Multi-feature) | 0.55 | 6.84 |

> ✅ **Gradient Boosting achieved the best performance**, indicating non-linear relationships between features and exam scores.  
> 💡 *It captured complex interactions — e.g., students with high motivation AND access to internet scored significantly higher than expected — revealing synergistic effects invisible to linear models.*

## 📌 Key Insights

- **Hours Studied** and **Teacher Quality** are the strongest predictors.
- **Parental involvement** and **access to resources** significantly impact outcomes.
- Gender showed negligible correlation → not a significant factor in this dataset.
- Target encoding improved performance for categorical variables like `School_Type`.
