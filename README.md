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


## 🛠 Data Preprocessing Workflow  

1. **Train/Test Split**  
   - The dataset was first split into **train** and **test** sets to prevent data leakage.  

2. **Handling Missing Values & Noise (Train Data)**  
   - Missing values in the training data were imputed using appropriate methods (median imputation or KNN-based imputation depending on the feature).  
   - Noisy values and outliers in the **train set** were detected and managed (either capped or removed).  

3. **Test Data Processing**  
   - The **test set** was **not used** for fitting preprocessing steps (to avoid leakage).  
   - Missing values in the test set were filled using the **median or KNN values derived from the training set**.  
   - Outliers in the test data were **not removed** to simulate real-world unseen data.  

4. **Feature Scaling**  
   - Scaling (StandardScaler / MinMaxScaler depending on the model) was **fitted only on the train data**.  
   - The same scaling transformation was then applied to the test data.  

✅ This ensures that all preprocessing is **train-data-driven**, and the test set remains a true unseen evaluation.  
