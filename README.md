Wine Quality Analysis and Classification
Project Overview

This project performs an end-to-end data analysis and machine learning workflow using the Wine Quality dataset, a widely used dataset in Data Science and Machine Learning.
The objective is to analyze physicochemical properties of wine and predict wine quality scores using a supervised classification model.

The project covers:

Exploratory Data Analysis (EDA)

Data cleaning and preprocessing

Feature scaling

Correlation analysis

Machine learning modeling with Random Forest

Model evaluation using standard classification metrics

Dataset Description

The dataset contains 1,143 observations of wine samples and includes 11 physicochemical features, one target variable (quality), and an identifier column (Id).

Features
Feature	Description
fixed acidity	Fixed acidity of the wine
volatile acidity	Volatile acidity, related to aroma
citric acid	Citric acid content
residual sugar	Amount of residual sugar
chlorides	Salt content
free sulfur dioxide	Free sulfur dioxide level
total sulfur dioxide	Total sulfur dioxide level
density	Wine density
pH	Acidity level
sulphates	Sulphate concentration
alcohol	Alcohol percentage
quality (target)	Wine quality score (0–10)
Id	Unique identifier

Target variable:
Although quality is numeric, it is treated as a categorical variable for classification.

Technologies and Libraries Used

Python

Pandas & NumPy – Data manipulation

Matplotlib & Seaborn – Data visualization

Scikit-learn – Machine learning and evaluation

Project Workflow
1. Data Loading

The dataset is loaded from a CSV file (WineQT.csv) and inspected using:

head()

info()

shape

describe()

This confirms:

No missing values

Correct data types

Expected dimensionality (1143 rows × 13 columns)

2. Exploratory Data Analysis (EDA)

Key EDA steps include:

Summary statistics for all numerical variables

Distribution analysis of the target variable (quality)

Visualization of class imbalance using bar charts

3. Data Cleaning

Missing values were checked using isnull()

No null values were found

A cleaned dataset was created using dropna() for completeness

4. Feature Scaling

To improve model performance:

All independent variables were normalized using StandardScaler

Scaling ensures features contribute equally to the model

Scaled data was converted back to a DataFrame for interpretability

5. Post-Scaling Visualization

Boxplots were used to visualize the distribution of selected normalized features

This confirms successful standardization and identifies potential outliers

6. Correlation Analysis

A correlation matrix was computed on normalized features

A heatmap was generated using Seaborn to identify:

Strong correlations

Redundant features

Relationships between physicochemical properties

Machine Learning Model
7. Train-Test Split

Dataset split into:

80% training

20% testing

Random seed set to ensure reproducibility

8. Model Training

RandomForestClassifier was selected due to:

Ability to handle nonlinear relationships

Robustness to feature scaling

Strong performance on tabular data

9. Model Evaluation

Evaluation metrics used:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

Results

Accuracy: ~69%

The model performs well for the most frequent quality classes (5 and 6)

Lower performance for rare classes (4 and 8), indicating class imbalance

Warnings related to undefined precision/recall are expected due to classes with no predicted samples.

10. Confusion Matrix

A confusion matrix was generated to:

Visualize prediction errors

Identify which quality classes are most frequently confused

Assess class-wise performance

Key Findings

Wine quality prediction is feasible using physicochemical properties

Class imbalance significantly impacts minority class performance

Random Forest provides reasonable baseline accuracy

Further improvements could include:

Class balancing techniques (SMOTE, class weights)

Hyperparameter tuning

Feature selection

Reframing the problem as regression

Future Improvements

Address class imbalance explicitly

Compare classification vs regression approaches

Optimize model hyperparameters

Add cross-validation

Evaluate feature importance in more depth

Author

Jonathan Bedoya
Data Analyst / BI / Product Data Analyst
