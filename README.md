![Project Banner](/c:/Users/benoi/.gemini/antigravity/brain/1c4840e4-22ae-478f-87df-d21a8fd15df3/titanic_project_banner_1767024661708.png)

# 🚢 Titanic Survival Prediction: Advanced ML Architecture

Welcome to the **Titanic Survival Prediction** project. This repository contains a production-grade data science workflow designed to predict passenger survival with high precision using advanced preprocessing, exhaustive hyperparameter optimization, and deep model interpretability.

> [!IMPORTANT]
> This project prioritizes **Quality over Speed**. It implements a rigorous 3-way data split (60/20/20) and advanced MICE imputation within an `ImbPipeline` to ensure zero data leakage and maximum reliability.

---

## 📊 Project Visuals & Logic

![Data Analysis Illustration](/c:/Users/benoi/.gemini/antigravity/brain/1c4840e4-22ae-478f-87df-d21a8fd15df3/data_analysis_illustration_1767024638719.png)

The core architecture follows a systematic journey from raw passenger data to a highly optimized voting ensemble.

---

## 🛠️ Technical Architecture

### 1. **Exhaustive Exploratory Data Analysis (EDA)**
Every feature underwent a granular investigation to uncover hidden patterns:
- **Survival Categorization**: Impact of Class, Sex, and Embarkation.
- **Missingness Heatmaps**: Identification of **MNAR** (Missing Not At Random) patterns in Age data.
- **Outlier Detection**: Distribution analysis for numerical features like Fare and Age.
- **Correlation Matrices**: Detailed mapping of feature influence on the target variable.

### 2. **Professional-Grade Preprocessing**
A robust pipeline was engineered to handle real-world data complexities:
- **Log Transformations**: Protecting the model from heavy-tailed outliers in `Fare`.
- **MICE Imputation**: Using iterative regression-based imputation for `Age` (fitted only on training data).
- **SMOTE**: Synthetic oversampling to address class imbalance during survival prediction.
- **Isolation Protocols**: All transformations are encapsulated in a `scikit-learn` Pipeline to prevent data leakage between training and validation sets.

### 3. **Modeling & Optimization**
We deploy a diverse set of "Artificial Intelligence" architectures:
- **Logistic Regression**: High-interpretability statistical baseline.
- **Random Forest**: Ensemble of trees for capture non-linear interactions.
- **XGBoost**: Gradient boosted decision trees for state-of-the-art accuracy.
- **Voting Ensemble**: A "Wisdom of the Crowds" model that combines all three for a more stable prediction.

> [!TIP]
> **Laptop-Optimized Tuning**: We run an exhaustive `GridSearchCV` that explores hundreds of parameter combinations (Depth, Learning Rate, Alpha, gamma) to maximize the **AUC (Area Under the Curve)**.

### 4. **Interpretability (SHAP Analysis)**
We don't just predict; we explain. Using **SHAP (SHapley Additive exPlanations)**, we decompose the "black box" models to see exactly how individual features like `Sex` or `Pclass` influenced each decimal of the final prediction.

---

## 🚀 Execution & Requirements

### Key Dependencies
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`, `xgboost`, `imblearn`
- `shap` (for model interpretability)

### How to Run
1. Ensure `Titanic-Dataset.csv` is in the project root.
2. Open `titanic_final_solution_v2.ipynb`.
3. Run all cells to execute the exhaustive EDA and model training.

---

## 🔮 Next Steps for Improvement
1. **Feature Interaction**: Deep dive into `Deck` and `Title` extraction from names.
2. **Advanced Stacking**: Implementing a meta-classifier on top of the current ensemble.
3. **Cross-Validation Scrutiny**: Increasing K-fold depth for even more robust parameter estimation.

---
*Created with ❤️ for Data Science Excellence.*
