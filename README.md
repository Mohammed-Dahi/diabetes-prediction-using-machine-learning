# Diabetes Prediction Using Machine Learning

A Machine Learning project that predicts whether a person is likely to have diabetes based on health and demographic information.

## Project Overview

This project focuses on building a Machine Learning classification system that predicts whether a person has diabetes using health-related and demographic features.

The project applies multiple classification algorithms, compares their performance, and selects the best-performing model based on test accuracy.

## Objective

The main objective is to develop an AI-based classification system that can predict diabetes using patient-related features such as:

* Age
* BMI
* Blood Glucose Level
* HbA1c Level
* Hypertension
* Heart Disease
* Smoking History
* Gender

## Dataset

**Dataset:** Diabetes Prediction Dataset
**Source:** Kaggle
**Kaggle Dataset:** `iammustafatz/diabetes-prediction-dataset`

### Dataset Information

* **Number of Records:** 96,146
* **Number of Features:** 8
* **Target Variable:** `diabetes`
* **Task:** Binary Classification

### Target Variable

* `0` → No Diabetes
* `1` → Diabetes

### Main Features

* `gender`
* `age`
* `hypertension`
* `heart_disease`
* `smoking_history`
* `bmi`
* `HbA1c_level`
* `blood_glucose_level`

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

### Workflow

```text
Kaggle Dataset
      ↓
Data Exploration
      ↓
Data Cleaning
      ↓
Data Preprocessing
      ↓
Train / Test Split
      ↓
Classification Models
      ↓
Model Evaluation
      ↓
Best Model Selection
```

## Data Exploration & Cleaning

The dataset was analyzed to understand its structure and identify potential data quality issues.

The following steps were performed:

* Checked dataset shape and structure
* Examined data types
* Checked for missing values
* Checked for duplicate records
* Examined the target variable distribution
* Checked possible invalid values
* Removed duplicate rows

## Exploratory Data Analysis

Several visualizations were created to understand the relationships between the features and diabetes.

The analysis focused on important health-related variables such as:

* Blood Glucose Level
* HbA1c Level
* Age
* BMI
* Hypertension
* Heart Disease

The analysis showed that **Blood Glucose Level** and **HbA1c Level** are particularly informative variables for diabetes prediction.

## Data Preparation

The dataset was divided into training and testing sets:

* **80% Training Data**
* **20% Testing Data**

### Numerical Features

The following preprocessing steps were applied:

* Missing values → Median Imputation
* Feature scaling → StandardScaler

### Categorical Features

The following preprocessing steps were applied:

* Missing values → Most-Frequent Imputation
* Encoding → One-Hot Encoding

A scikit-learn preprocessing pipeline was used to keep the preprocessing steps organized and reduce the risk of data leakage.

## Machine Learning Models

Four classification algorithms were trained and evaluated:

### 1. Logistic Regression

A simple and interpretable classification algorithm used as one of the baseline models.

### 2. Decision Tree

A tree-based classification model that makes predictions using a sequence of decision rules.

### 3. Random Forest

An ensemble learning algorithm that combines multiple decision trees to improve predictive performance.

### 4. K-Nearest Neighbors (KNN)

A classification algorithm that predicts the class of a data point based on the classes of nearby observations.

## Model Evaluation

The primary evaluation metric used to compare the models was **Accuracy**.

### Accuracy

```text
Accuracy = Correct Predictions / Total Predictions
```

In addition to Accuracy, the final model was evaluated using:

* Classification Report
* Precision
* Recall
* F1-Score
* Confusion Matrix

## Results

The four models were evaluated on the test dataset.

| Model                     | Test Accuracy |
| ------------------------- | ------------: |
| **Random Forest**         |    **96.92%** |
| Logistic Regression       |        95.96% |
| K-Nearest Neighbors (KNN) |        95.93% |
| Decision Tree             |        94.79% |

### Best Performing Model

**Random Forest**

### Test Accuracy

**96.92%**

The Random Forest model achieved the highest test accuracy among all evaluated classification models.

### Classification Report

For the **Diabetes** class (`1`):

* **Precision:** 95%
* **Recall:** 69%
* **F1-Score:** 80%

The Classification Report and Confusion Matrix were also used to provide a more complete evaluation beyond Accuracy.

## Key Findings

The main findings from the project include:

* Random Forest achieved the highest test accuracy.
* The final test accuracy was **96.92%**.
* Blood Glucose Level is an important variable for diabetes prediction.
* HbA1c Level is also a highly informative health indicator.
* Age and BMI can provide additional predictive information.
* Comparing multiple classification algorithms helped identify the best-performing model.
* Accuracy alone does not provide a complete picture of classification performance, so Precision, Recall, and F1-Score were also considered.

## Future Improvements

The project can be improved further by:

* Applying Hyperparameter Tuning
* Using Cross-Validation
* Testing additional classification algorithms
* Performing Feature Importance Analysis
* Optimizing Precision, Recall, and F1-Score
* Handling class imbalance more extensively
* Deploying the final model as a Web Application

## Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **KaggleHub**
* **Google Colab**
* **Jupyter Notebook**

## Project Files

```text
diabetes-prediction-using-machine-learning/
│
├── Diabetes_Prediction_Final_Project.ipynb
├── Presentation.pptx
├── README.md
├── requirements.txt
└── .gitignore
```

### File Description

* `Diabetes_Prediction_Final_Project.ipynb` → Complete Machine Learning project and analysis
* `Presentation.pptx` → Project presentation
* `README.md` → Project documentation
* `requirements.txt` → Required Python libraries
* `.gitignore` → Files excluded from GitHub

## How to Run

### Google Colab

1. Open `Diabetes_Prediction_Final_Project.ipynb` in Google Colab.
2. Run the cells from top to bottom.
3. The dataset is loaded using KaggleHub.
4. Review the data analysis, visualizations, model comparison, and final results.

### Local Environment

Install the required libraries:

```bash
pip install -r requirements.txt
```

Then open the notebook:

```text
Diabetes_Prediction_Final_Project.ipynb
```

## Disclaimer

This project is developed for **educational and Machine Learning practice purposes only**.

It is **not a medical diagnostic tool** and should not be used to make clinical decisions.

## Author

**Mohammed Dahi**

Machine Learning & Data Analysis Final Project
