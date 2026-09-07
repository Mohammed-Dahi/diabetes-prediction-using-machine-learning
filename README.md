# Diabetes Prediction Using Machine Learning

## Project Overview

This project focuses on building a Machine Learning system that predicts whether a person has diabetes based on health and demographic information.

The project applies several classification algorithms, compares their performance, and selects the best-performing model based on test accuracy.

## Objective

The main objective is to develop an AI-based classification system that can predict diabetes using patient-related features such as age, BMI, blood glucose level, HbA1c level, hypertension, heart disease, and smoking history.

## Dataset

**Dataset:** Diabetes Prediction Dataset
**Source:** Kaggle
**Task:** Binary Classification

### Target Variable

* `0` → No Diabetes
* `1` → Diabetes

### Main Features

* Gender
* Age
* Hypertension
* Heart Disease
* Smoking History
* BMI
* HbA1c Level
* Blood Glucose Level

## Project Workflow

The project follows these main steps:

1. Data Loading
2. Data Exploration
3. Data Cleaning
4. Exploratory Data Analysis
5. Data Preprocessing
6. Train-Test Split
7. Classification Model Training
8. Model Evaluation
9. Best Model Selection

## Data Cleaning & Preprocessing

The dataset was analyzed and prepared before applying Machine Learning models.

The preprocessing steps included:

* Checking missing values
* Checking duplicate records
* Removing duplicate rows
* Checking possible invalid values
* Separating features and target
* Splitting the data into training and testing sets
* Handling numerical features
* Handling categorical features
* Feature scaling
* One-hot encoding

An 80/20 train-test split was used.

## Machine Learning Models

Four classification algorithms were tested:

### Logistic Regression

A simple and interpretable classification algorithm.

### Decision Tree

A tree-based model that makes predictions using decision rules.

### Random Forest

An ensemble learning algorithm that combines multiple decision trees.

### K-Nearest Neighbors (KNN)

A classification algorithm that predicts based on the most similar observations.

## Model Evaluation

The main evaluation metric used in this project is **Accuracy**.

The models were compared using their performance on the test dataset.

Additional evaluation methods include:

* Classification Report
* Confusion Matrix
* Accuracy Comparison

The model with the highest test accuracy was selected as the final model.

## Key Findings

The exploratory analysis showed that several health-related variables can provide useful information for diabetes prediction.

Important features include:

* Blood Glucose Level
* HbA1c Level
* Age
* BMI
* Hypertension
* Heart Disease

Among these variables, blood glucose and HbA1c levels are particularly important indicators in the analysis.

## Results

The final model and its exact test accuracy are generated directly from the executed notebook.

**Best Model:** [Add the best model from the notebook]

**Test Accuracy:** [Add the final accuracy from the notebook]

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* KaggleHub
* Google Colab
* Jupyter Notebook

## Future Improvements

Future improvements could include:

* Hyperparameter tuning
* Cross-validation
* Testing additional Machine Learning algorithms
* Feature importance analysis
* Using Precision, Recall, and F1-score
* Deploying the model as a web application

## Project Files

* `Diabetes_Prediction_Final_Project.ipynb` → Complete project notebook
* `README.md` → Project documentation
* `requirements.txt` → Required Python libraries
* `.gitignore` → Files excluded from GitHub

## Disclaimer

This project is developed for educational and Machine Learning practice purposes only. It is not a medical diagnostic tool and should not be used to make clinical decisions.

## Author

**Mohammed Dahi**

Machine Learning & Data Analysis Project
