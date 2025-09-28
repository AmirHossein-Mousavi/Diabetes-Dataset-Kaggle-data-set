Dataset

Dataset: https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset

Samples: 768

Features: 8 medical predictor variables

Target: Outcome (0 = No Diabetes, 1 = Diabetes)

⚡ Workflow

1.Data Preprocessing

*Handling missing values

*Feature scaling (StandardScaler)

*Train/test split

2.Model Training & Tuning

*Logistic Regression

*Decision Tree

*Random Forest

*XGBoost

*LightGBM

*Support Vector Machine (SVM)

*Multi-layer Perceptron (MLP)


✅ Hyperparameter tuning with GridSearchCV / RandomizedSearchCV

✅ Models saved using joblib

-----------------------------------------------------------------------------------

*** Evaluation

Metrics: Accuracy, F1-score, ROC-AUC

Confusion matrices & classification reports

Feature importance (for tree models)

*** Ensemble Methods

Soft Voting (but i tested Weighted Voting (based on Test F1-score) and it was not really effective)

*** Visualization

Bar plots for performance comparison

ROC curves for all models

Confusion matrices

Feature importance plots


## 📊 Results  

| Model               | Train Accuracy | Test Accuracy | Train F1 | Test F1 | Test ROC-AUC |
|----------------------|----------------|---------------|----------|---------|--------------|
| Random Forest        | 0.853 | 0.747 | 0.806 | 0.693 | 0.822 |
| LightGBM             | 0.802 | 0.721 | 0.741 | 0.672 | 0.819 |
| SVM                  | 0.740 | 0.682 | 0.674 | 0.642 | 0.798 |
| XGBoost              | 0.908 | 0.727 | 0.852 | 0.611 | 0.809 |
| MLP                  | 0.802 | 0.721 | 0.667 | 0.598 | 0.801 |
| Logistic Regression  | 0.797 | 0.708 | 0.650 | 0.571 | 0.811 |
| Decision Tree        | 0.867 | 0.695 | 0.802 | 0.535 | 0.716 |
| **Voting Ensemble**  | 0.855 | 0.714 | 0.775 | 0.600 | 0.807 |
| **Weighted Voting**  | 0.855 | 0.714 | 0.775 | 0.610 | 0.820 |

