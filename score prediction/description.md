# Score Prediction Project

This folder contains a comprehensive machine learning pipeline designed to analyze and predict student performance based on various demographic, social, and academic factors.

## Folder Overview
The `score prediction` folder serves as the main workspace for student performance analysis. It integrates multiple datasets (spanning over 1,000 students) and a central Jupyter Notebook that performs end-to-end data science tasks, from exploratory data analysis (EDA) to advanced regression modeling.

## Files Description

### 1. `Student_Performance_Analysis.ipynb`
The core of the project. This Jupyter Notebook contains the entire machine learning workflow, including:
- **Data Preprocessing**: Handling categorical variables and scaling features.
- **Exploratory Data Analysis (EDA)**: Visualizing trends and correlations between student habits and their final scores.
- **Model Training**: Implements 10 different regression models, including Linear Regression, Tree-based models (Decision Trees, Random Forests), and Ensemble methods (Gradient Boosting, XGBoost).
- **Scenario Analysis**: Evaluates prediction accuracy in two conditions:
  - *With intermediate grades*: Achieving a high R² of ~82.7%.
  - *Without intermediate grades*: Focusing on socio-economic predictors (R² ~23.1%).
- **Optimization**: Hyperparameter tuning and feature importance analysis (identifying "absences" and "previous failures" as top predictors).

### 2. `StudentsPerformance.csv`
A dataset containing 1,000 student records with the following attributes:
- **Demographics**: Gender, race/ethnicity.
- **Background**: Parental level of education, lunch type (standard vs. free/reduced), and test preparation course completion.
- **Target Metrics**: Math, reading, and writing scores.

### 3. `student-mat.csv`
A specialized dataset focusing on student performance in **Mathematics**. 
- **Sample Size**: ~395 students.
- **Features**: Includes school-specific data, family size, study time, alcohol consumption (daily/weekend), and three-period grades (G1, G2, G3).
- **Format**: Semicolon-separated values.

### 4. `student-por.csv`
A specialized dataset focusing on student performance in the **Portuguese language** course.
- **Sample Size**: ~649 students.
- **Features**: Mirrors the structure of `student-mat.csv`, providing a cross-subject comparison for behavioral features.
- **Format**: Semicolon-separated values.

### 5. `description.md`
This file provides a structured guide to the contents and objectives of the score prediction module.
