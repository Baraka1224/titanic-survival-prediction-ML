# Titanic Survival Prediction Project 

This project applies supervised machine learning models to predict passenger survival from the Titanic disaster. It uses structured data from Kaggle and includes preprocessing, model evaluation, feature importance analysis, and interpretability with SHAP values.


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

##  Preprocessing

- Imputation (median for Age/Fare)
- One-hot encoding (for categorical variables)
- Z-score normalization (for numerical variables)
  
 ## Hyperparameter Tuning
GridSearchCV with 3-fold cross-validation was used to optimize:
- `max_depth` and `n_estimators` for Random Forest  
- `max_depth` for Decision Tree

##  Results

- Best Model: **Random Forest**
- Accuracy: **83.1%**
- ROC-AUC: **0.87**
- Key predictors: **Fare, Sex, Age**
