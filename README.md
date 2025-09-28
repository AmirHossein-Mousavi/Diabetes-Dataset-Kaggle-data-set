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

📊 Results
Model             	Train Acc   -   	Test Acc	 -   Train F1	  -   Test F1	  -   Test ROC-AUC

Random Forest	        0.85	    -       0.74	   -   0.81	      -     0.69	  -        0.82

LightGBM	            0.80      -     	0.72	   -   0.74       -   	0.67    -     	 0.82

SVM                  	0.74      -      	0.68     -  	0.67      -   	0.64    -     	 0.80

XGBoost	              0.91	    -       0.73	   -    0.85	    -     0.61	  -        0.81

MLP	                  0.80	    -       0.72	   -    0.67	    -     0.60	  -        0.80

Logistic Regression	  0.79	    -       0.71	   -    0.65	    -     0.57	  -        0.81

Decision Tree        	0.86	    -       0.69	   -    0.80	    -     0.53	  -        0.71

Voting Ensemble	      0.85	    -       0.71	   -    0.77	    -     0.60	  -        0.81

Weighted Voting	      0.85	    -       0.71	   -    0.77	    -     0.61	  -        0.82

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

