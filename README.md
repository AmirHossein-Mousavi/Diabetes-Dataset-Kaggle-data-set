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
