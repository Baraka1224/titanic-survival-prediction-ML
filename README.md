## Titanic Survival Prediction – Machine Learning Project

This project applies supervised machine learning to predict passenger survival from the Titanic disaster using structured data. It was developed as part of a final academic project to demonstrate real-world application of data science principles, including model selection, preprocessing, evaluation, and interpretation.


##  Overview

This project uses the [Kaggle Titanic dataset](https://www.kaggle.com/competitions/titanic) to classify whether a passenger survived based on features such as:
- Age
- Sex
- Passenger Class (Pclass)
- Fare
- Number of siblings/spouses aboard (SibSp)
- Number of parents/children aboard (Parch)
- Embarked location

Three models were compared:
- **Logistic Regression**
- **Decision Tree**
- **Random Forest** (best performer)

---

##  Dataset

- Source: [Kaggle Titanic ML Challenge](https://www.kaggle.com/competitions/titanic)
- Total records: 891 passengers
- Target variable: `Survived` (0 = No, 1 = Yes)

---

##  Data Preprocessing

- **Missing Values:**  
  - Age and Fare: Filled using median values  
  - Embarked: Filled using mode (`'S'`)

- **Encoding:**  
  - One-hot encoding for categorical features: `Sex`, `Embarked`

- **Feature Scaling:**  
  - Z-score normalization applied to `Age` and `Fare`

- **Split:**  
  - 75% training, 25% testing

---

##  Models Used

| Model               | Description                              |
|--------------------|------------------------------------------|
| Logistic Regression| Simple and interpretable baseline model  |
| Decision Tree       | Captures non-linear splits               |
| Random Forest       | Ensemble model with highest performance |

---

##  Hyperparameter Tuning

- **GridSearchCV** used with 3-fold cross-validation.
- Best parameters:
  - `Random Forest`: `max_depth=4`, `n_estimators=50`
  - `Decision Tree`: `max_depth=2`

---

##  Evaluation Metrics

| Model               | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|--------------------|----------|-----------|--------|----------|---------|
| Logistic Regression| 80.3%    | 0.76      | 0.73   | 0.74     | 0.84    |
| Decision Tree       | 77.9%    | 0.73      | 0.71   | 0.72     | 0.80    |
| Random Forest       | 83.1%    | 0.79      | 0.77   | 0.78     | 0.87    |

---

## Visualizations

Key visuals used to interpret the models:
- Correlation matrix
- Feature importance (Random Forest)
- Confusion matrix
- ROC curve

All visuals are included in the `figures/` folder of this repository.

---

## Reflections

This project helped me build a complete ML pipeline from data exploration to evaluation and interpretation. I focused on visual tools like feature importance and ROC curves to support interpretability.

###  What I Learned:
- The importance of data cleaning before modeling
- The value of comparing multiple models
- How to interpret confusion matrices and ROC curves
- The impact of peer feedback on improving analysis

### Peer Feedback Incorporated:
- Added more visualizations (correlation matrix, confusion matrix)
- Clarified data split and hyperparameter tuning process
- Removed typos and improved flow in written report

---

