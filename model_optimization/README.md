# Diabetes Prediction - Random Forest Hyperparameter Optimization

This subproject focuses on optimizing a Random Forest model for predicting diabetes using patient health data. The model is fine-tuned using GridSearchCV to identify the best combination of hyperparameters for improved performance.

---

## 📌 Objective
To improve the F1-score and recall of the diabetes prediction model, especially for identifying diabetic patients (Class 1).

---

## ⚙️ Methodology

- **Dataset**: Pima Indians Diabetes dataset
- **Algorithm**: Random Forest Classifier
- **Tuning Method**: GridSearchCV
- **Scoring Metric**: F1-Score (with 5-fold cross-validation)

### 🔍 Hyperparameters Tuned:
- `n_estimators`: 200  
- `max_depth`: 5  
- `min_samples_split`: 5  
- `min_samples_leaf`: 2

---

## 📈 Results

### 🔹 Best Model Performance
- **Accuracy**: 76%
- **F1-Score (Diabetic Class)**: 0.70
- **ROC AUC Score**: 0.768
- **Recall (Diabetic Class)**: 80%
- **Precision (Diabetic Class)**: 63%

### 🔹 Confusion Matrix:
          Predicted
          0     1

---

### 🔹 Top 3 Most Important Features:
1. Glucose
2. BMI
3. Age

(As shown in the feature importance plot)

---

## 📁 Files

| File | Description |
|------|-------------|
| `rf_hyperparameter_tuning.ipynb` | Jupyter Notebook with full tuning workflow |
| `feature_importance_plot.png` | Feature importance bar chart |
| `diabetes.csv` | Dataset used for training and testing |

---

## 🚀 Next Steps

- Compare performance with other classifiers (e.g., XGBoost, SVM)
- Perform feature engineering (e.g., BMI ranges)
- Explore recall boosting methods (e.g., SMOTE for class imbalance)

---

## 🧪 Built With

- Python 3.10
- Scikit-learn
- Seaborn & Matplotlib
- GridSearchCV
- Pandas & NumPy
