# Machine-Learning-Pipeline-for-Parkinson-s-Disease-Detection
A complete pipeline that explores biomedical voice features, performs preprocessing, and trains multiple models (Logistic Regression, Random Forest, SVM) with hyperparameter tuning. Includes evaluation with accuracy, ROC AUC, confusion matrix, and model saving for deployment.

This project builds a machine learning pipeline to detect Parkinson’s disease from biomedical voice features.
It includes data preprocessing, exploratory analysis, model training (Logistic Regression, Random Forest, SVM), hyperparameter tuning with cross-validation, evaluation, and model saving for deployment.

Project Structure

├── parkinsons.csv                  
├── parkinsons_ml_pipeline_v2.py    
├── notebooks/                                           
└── README.md

                      

**Features:**

Loads and cleans the Parkinson’s dataset (drops irrelevant columns, handles missing values).

Exploratory Data Analysis (summary statistics, missing values, correlation heatmap).

Train/test split with stratification to preserve class balance.

Machine Learning Models:

Logistic Regression

Random Forest

Support Vector Machine (SVM)

Hyperparameter tuning with GridSearchCV and cross-validation.

Evaluation metrics: Accuracy, ROC AUC, Cohen’s Kappa, Confusion Matrix, Classification Report.

Saves the best trained model (.joblib) and performance reports for reuse.



**Dataset :**

Source: UCI Machine Learning Repository – Parkinson’s Disease Data Set

Rows: 195

Columns: 24 (22 features, 1 ID, 1 target)

Target column: status

1 → Patient has Parkinson’s disease

0 → Patient is healthy




**Installation:**

Clone the repository and install dependencies:

git clone https://github.com/your-username/parkinsons-detection.git
cd parkinsons-detection




**Example Results:**

From one test run:

Accuracy: 92.3%

ROC AUC: 0.96

Cohen’s Kappa: 0.79

Very high recall for detecting Parkinson’s patients (97%).

Confusion Matrix:

Predicted Healthy   Predicted Sick
Healthy        8             2
Sick           1            28
