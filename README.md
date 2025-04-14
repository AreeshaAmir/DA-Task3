Fraud Detection System

1. Overview

This project builds a fraud detection system using machine learning to classify credit card transactions as fraudulent (1) or legitimate (0).

The dataset used is creditcard.csv, which contains transaction records.

2. Steps Performed

2.1 Data Preprocessing

Loaded the dataset and separated features (X) and the target variable (y).

Standardized features using StandardScaler to normalize the data.

Handled class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).

Split the dataset into training (80%) and testing (20%) subsets.

2.2 Model Training

Used Random Forest Classifier with 100 trees.

Trained the model on the resampled dataset.

2.3 Model Evaluation

Predicted fraud using the test dataset.

Calculated key performance metrics:

Accuracy

Precision

Recall

F1-score

Confusion Matrix (Plotted using Seaborn)

2.4 Feature Importance Analysis

Extracted feature importance from the trained model.

Displayed the top 10 features contributing to fraud detection.

2.5 Fraud Detection CLI (Command Line Interface)

Loads a trained model and scaler.

Uses a sample transaction for testing.

Predicts if the transaction is fraudulent or legitimate.

3. Output Example

Model Evaluation:

Accuracy: 0.9845

Precision: 0.9567

Recall: 0.9210

F1-score: 0.9385

Confusion Matrix:

[[ 56890    112]
 [   48    290]]

Feature Importance Ranking:

V17: 0.1923

V12: 0.1347

V10: 0.1215

...

Fraud Detection System - Test with Sample Transaction

🚨 Fraudulent Transaction Detected!


4. How to Run the Code?

Install required libraries:

pip install pandas numpy scikit-learn imbalanced-learn seaborn matplotlib joblib

Run the script:

python fraud_detection.py
View model evaluation and fraud detection results.
