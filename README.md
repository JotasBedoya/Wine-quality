Wine Quality Classification – Machine Learning Pipeline

Python + Scikit-learn + Pandas + Seaborn

🎯 Objective
This project builds an end-to-end machine learning classification pipeline to predict wine quality based on physicochemical properties.
It showcases core Data Analysis and Machine Learning skills commonly required for Data Analyst and Data Scientist roles.

🧩 Problem Statement
The wine dataset contains multiple chemical attributes, but without analysis it is difficult to:

Understand which features influence wine quality

Identify correlations between physicochemical variables

Predict wine quality consistently

Evaluate model performance across different quality classes

This results in limited insight into quality drivers and predictive capability.

🚀 Solution Architecture

RAW CSV Dataset
→ Exploratory Data Analysis (EDA)
→ Data Cleaning & Feature Scaling
→ Correlation Analysis
→ Train/Test Split
→ Random Forest Classification Model
→ Model Evaluation (Accuracy, Report, Confusion Matrix)

🏗️ Tech Stack

Layer	Tool
Data Processing	Python, Pandas, NumPy
Visualization	Matplotlib, Seaborn
Machine Learning	Scikit-learn
Modeling	RandomForestClassifier
Version Control	GitHub

📂 Repository Structure

wine-quality-classification/
│── datasets/
│   └── WineQT.csv
│── notebooks/
│   └── wine_quality_analysis.ipynb
│── README.md


🧮 Model Output & Evaluation

Target: Wine quality score (0–10, treated as categorical)

Accuracy: ~69%

Strong performance on majority classes (quality 5 and 6)

Lower recall for minority classes due to class imbalance

Evaluation methods:

Accuracy score

Classification report

Confusion matrix

📊 Key Insights

Alcohol, sulphates, and acidity show meaningful relationships with quality

Class imbalance impacts minority quality predictions

Random Forest provides a solid baseline for classification tasks

🔧 Future Improvements

Apply class balancing techniques (SMOTE, class weights)

Hyperparameter tuning

Compare classification vs regression approaches

Feature importance analysis

📌 Author
Jonathan Bedoya
Data Analyst | BI Developer | Analytics-Focused ML
LinkedIn: https://www.linkedin.com/in/jonathanbedoya1993
