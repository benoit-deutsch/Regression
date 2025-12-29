![Cutty Sark in Greenwich](assets/cutty_sark.png)

# 🚢 Titanic Survival Prediction: Antigravity Use case

This entire repository—including the exhaustive EDA, the robust machine learning pipelines, the hyperparameter optimization scripts, and this documentation - was engineered by **Antigravity**. It serves as an example of autonomous AI usage in data engineering and predictive modeling tasks.

---

## 🛠️ Technical Architecture 

### 🛡️ Professional Preprocessing
We implement a robust pipeline that prevents data leakage by isolating training and validation data:
- **MICE Imputation**: Iterative regression-based logic for filling missing `Age` values.
- **SMOTE**: Synthetic oversampling to handle target class imbalance.
- **Log Scaling**: Transforming the `Fare` feature to mitigate outlier impact.

### 🧠 Modeling & Optimization
We deploy a diverse set of AI architectures, fine-tuned on your local hardware:
- **Logistic Regression**: Optimized for both L1 and L2 regularization.
- **Random Forest**: Exhaustive search over tree depth, feature sampling, and leaf constraints.
- **XGBoost**: Gradient boosted trees tuned for maximum AUC with precise gamma and subsample control.
- **Voting Ensemble**: A soft-voting powerhouse combining the strengths of all individual models.

### 🔍 Explanability (SHAP)
Predictive accuracy is paired with deep interpretability. By utilizing **SHAP (SHapley Additive exPlanations)**, the project uncovers the specific feature influences behind every prediction, transforming "black box" logic into readable insights.

---

## 🚀 How to Run
1. Ensure `Titanic-Dataset.csv` is in the project root.
2. Open `titanic.ipynb`.
3. Run all cells to execute the full pipeline from raw data to ensemble evaluation.
