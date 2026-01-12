Wine Quality Classification
Overview

This project analyzes the Wine Quality dataset and builds a machine learning classification model to predict wine quality based on physicochemical properties. The workflow covers data exploration, preprocessing, feature scaling, correlation analysis, and model evaluation.

Dataset

Samples: 1,143 wines

Features: 11 physicochemical variables

Target: quality (0–10, treated as categorical)

Key features include acidity levels, sugar, sulphates, alcohol, pH, and density.

Tools & Libraries

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

Workflow

Data loading and inspection

Exploratory Data Analysis (EDA)

Data cleaning (no missing values)

Feature scaling with StandardScaler

Correlation analysis (heatmap)

Train/Test split (80/20)

Model training using RandomForestClassifier

Evaluation with accuracy, classification report, and confusion matrix

Model Performance

Accuracy: ~69%

Strong performance on majority classes (quality 5 and 6)

Lower recall on minority classes due to class imbalance

Key Takeaways

Wine quality can be reasonably predicted using physicochemical features

Class imbalance impacts minority class performance

Random Forest provides a solid baseline model

Future Improvements

Handle class imbalance (e.g., SMOTE or class weights)

Hyperparameter tuning

Compare classification vs regression approaches

Author

Jonathan Bedoya
Data Analyst / BI / Product Data Analyst
