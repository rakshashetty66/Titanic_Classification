# Titanic Survival Prediction System
1. This project builds a machine learning model to predict whether a passenger on the Titanic would survive the disaster.
2. The model leverages multiple personal and socio-economic factors, such as age, gender, class, and family size, to make the prediction.
3. It also provides insights into which factors most strongly influenced survival chances.

# Table of Contents
Introduction

Dataset

Methodology

Feature Engineering

Model Selection

Evaluation

Feature Importance

Setup and Installation

Usage

Results and Insights

# Introduction
The Titanic Survival Prediction System uses various machine learning algorithms to predict whether a passenger on the Titanic would have survived. 

This project is a classic example of binary classification and explores factors influencing survival, such as socio-economic status, age, and gender.

# Dataset

This project uses the Titanic dataset from Kaggle, which includes the following attributes:

1. Pclass: Ticket class (1st, 2nd, or 3rd)
2. Sex: Gender of the passenger
3. Age: Age of the passenger
4. SibSp: Number of siblings/spouses aboard
5. Parch: Number of parents/children aboard
6. Fare: Ticket fare
7. Embarked: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)

Additional attributes like Name, Ticket, and Cabin are used for feature engineering.

# Methodology

The project follows a structured approach:

1. Data Preprocessing: Handle missing values and encode categorical variables.
2. Feature Engineering: Create new features such as FamilySize and Title to provide more insights for the model.
3. Feature Selection: Identify features most relevant to survival, including socio-economic status, age, gender, and family size.

# Feature Engineering

1. Family Size: Calculated by adding SibSp and Parch to indicate family support, which might influence survival.
2. Title Extraction: Titles (e.g., Mr., Miss, Mrs.) are extracted from the Name column, representing social status.

# Model Selection

The following machine learning models are evaluated:

1. Logistic Regression: A simple binary classifier suitable for this task.
2. Random Forest: An ensemble model that helps identify feature importance.
3. Decision Tree: Useful for non-linear relationships.
4. Support Vector Machine (SVM): Effective for complex datasets.
5. K-Nearest Neighbors (KNN): A distance-based classifier.

Each model is trained on the preprocessed data and evaluated to find the best-performing model.

# Evaluation

Models are evaluated using:

1. Accuracy Score: Measures correct predictions as a percentage.
2. Classification Report: Provides precision, recall, and F1-score for each model.
3. Confusion Matrix: Displays true positives, false positives, false negatives, and true negatives.
4. Cross-Validation: Helps validate the consistency of model performance.

# Feature Importance

Using the Random Forest model, feature importance is analyzed to understand the impact of each factor on survival probability. Key factors include:

1. Gender: Females had a higher survival rate.
2. Class: Higher ticket classes (1st and 2nd) increased survival chances.
3. Age: Younger passengers, especially children, were more likely to survive.
4. Family Size: Passengers with moderate family sizes showed higher survival likelihood.


