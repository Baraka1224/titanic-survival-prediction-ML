# Titanic Survival Prediction Project 

This project applies supervised machine learning models to predict passenger survival from the Titanic disaster. It uses structured data from Kaggle and includes preprocessing, model evaluation, feature importance analysis, and interpretability with SHAP values.

##  Contents

- `titanic_analysis.ipynb` — Jupyter Notebook with all modeling steps and visualizations
- `figures/` — folder with correlation matrix, ROC curve, confusion matrix, and feature importance plots
- `final_report.docx` — academic paper version of the project
- `requirements.txt` — list of Python libraries used

##  Models Used

- Logistic Regression  
- Decision Tree  
- Random Forest (best performance)

##  Evaluation Metrics

- Accuracy, Precision, Recall, F1-score
- ROC-AUC
- Confusion Matrix
- Feature Importance
- Correlation Matrix

##  SHAP Explainability

SHAP values were used to understand model decisions and improve transparency.

##  Preprocessing

- Imputation (median for Age/Fare)
- One-hot encoding (for categorical variables)
- Z-score normalization (for numerical variables)

##  Results

- Best Model: **Random Forest**
- Accuracy: **83.1%**
- ROC-AUC: **0.87**
- Key predictors: **Fare, Sex, Age**
