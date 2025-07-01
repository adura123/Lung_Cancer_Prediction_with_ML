# Lung_Cancer_Prediction_with_ML
Predicting lung cancer risk levels using machine learning models. Compares Logistic Regression, Gaussian Naïve Bayes, and Multinomial Naïve Bayes for early diagnosis and improved patient outcomes.
Project Overview
Lung cancer is one of the leading causes of death globally, with over 2.2 million cases diagnosed in 2020. Early detection is critical for improving survival rates, but traditional screening methods are limited. Machine learning (ML) provides an opportunity to enhance predictive accuracy and early risk identification through automated analysis of complex datasets.

🧠 Objectives
Predict lung cancer risk levels (High, Medium, Low) using ML.

Compare three classifiers: Logistic Regression, Gaussian Naïve Bayes, and Multinomial Naïve Bayes.

Evaluate and improve model performance through hyperparameter tuning and K-Fold Cross Validation.

Demonstrate how ML can support early detection and decision-making in clinical settings.

📊 Dataset
Source: Kaggle - Lung Cancer Dataset

Records: 1000 samples

Features: 26 (25 numerical, 1 categorical)

Target variable: Level

0 = Low Risk

1 = Medium Risk

2 = High Risk

⚙️ Methodology
1. Data Preprocessing
Dropped irrelevant columns (Index, Patient ID)

Converted categorical values to numerical

Normalized data using Min-Max Scaling

Verified class distribution – no rebalancing required

2. Models Used
Logistic Regression

Best performance overall

Tuned hyperparameters: C=10, penalty='l1', solver='liblinear'

Gaussian Naïve Bayes

Fast and effective for smaller datasets

Assumes features follow a Gaussian distribution

Multinomial Naïve Bayes

Typically for text/NLP data

Included for comparative purposes

3. Performance Evaluation
K-Fold Cross Validation

ROC Curve

Metrics Used:

Accuracy

Precision

Recall

AUC (Area Under the Curve)

📈 Results
Model	Accuracy	Precision	Recall	Tuned Accuracy	CV Accuracy
Logistic Regression	0.97	0.98	0.97	1.00	1.00
Gaussian Naïve Bayes	0.88	0.88	0.88	0.89	0.89
Multinomial Naïve Bayes	0.70	0.71	0.70	0.70	0.70

Logistic Regression outperformed other models in all evaluation metrics.

ROC curves confirmed high separability of logistic regression predictions.

K-Fold CV validated the generalizability of the results.

📌 Conclusion
Logistic Regression is the most effective model for predicting lung cancer risk levels, with perfect classification after hyperparameter tuning. Gaussian Naïve Bayes also shows strong performance and is suitable for quick, probabilistic classification tasks. This work underscores how ML can be applied effectively for early diagnosis and clinical risk assessment in healthcare.

🔧 Technologies Used
Python

pandas, numpy

scikit-learn

seaborn, matplotlib

Jupyter Notebook
