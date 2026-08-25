# Codveda Machine Learning Internship

This file contains the machine learning tasks completed during my internship at **Codveda Technologies**.

The main objective of these projects is to practice the complete machine learning workflow, including data preprocessing, model training, prediction, evaluation, and interpretation.

## Project Structure

```text
Codveda_Machine_Learning/
│
├── level_1/
│   ├── task_1_data_preprocessing/
│   └── task_2_linear_regression/
│
├── level_2/
│   └── task_1_logistic_regression/
│
└── README.md
```

## Level 1 – Task 1: Data Preprocessing

In this task, I prepared a stock price dataset for machine learning.

### Work Completed

* Loaded and explored the dataset using Pandas.
* Identified missing values.
* Removed rows containing missing values.
* Identified categorical and numerical features.
* Encoded categorical data.
* Converted the date column into useful numerical features.
* Split the dataset into training and testing sets.
* Applied standardization using `StandardScaler`.
* Avoided data leakage by fitting the scaler only on the training data.

### Main Concepts Learned

* Missing value handling
* Data exploration
* Categorical encoding
* Feature scaling
* Train/Test split
* Data leakage prevention

---

## Level 1 – Task 2: Linear Regression

In this task, I developed a Linear Regression model using a house prediction dataset.

### Work Completed

* Loaded and explored the dataset.
* Separated the input features (`X`) from the target (`y`).
* Split the data into training and testing sets.
* Created and trained a Linear Regression model.
* Generated predictions on unseen test data.
* Compared actual and predicted values.
* Evaluated the model using:

  * Mean Squared Error (MSE)
  * R² Score
* Analyzed the model coefficients and intercept.
* Visualized actual versus predicted values.

### Main Concepts Learned

* Regression problems
* Features and target variables
* Model training using `fit()`
* Prediction using `predict()`
* Linear Regression coefficients
* MSE
* R² Score
* Model evaluation

---

## Level 2 – Task 1: Logistic Regression

In this task, I developed a Logistic Regression model for customer churn prediction.

The objective was to predict whether a customer would leave the service.

### Work Completed

* Loaded separate training and testing datasets.
* Explored the customer churn data.
* Converted the target from Boolean values to binary values:

  * `False → 0`
  * `True → 1`
* Applied One-Hot Encoding to categorical features.
* Applied feature standardization.
* Trained a Logistic Regression model.
* Generated class predictions.
* Generated churn probabilities using `predict_proba()`.
* Evaluated the model using:

  * Accuracy
  * Precision
  * Recall
  * Confusion Matrix
  * Classification Report
  * ROC Curve
  * AUC Score
* Analyzed model coefficients and odds ratios.

### Model Results

* Accuracy: **85.46%**
* Precision: **47.73%**
* Recall: **22.11%**
* AUC: **81.38%**

The results showed that accuracy alone is not enough to evaluate an imbalanced classification problem. Precision, Recall, ROC, and AUC provide additional information about the model's performance.

### Main Concepts Learned

* Binary Classification
* Logistic Regression
* One-Hot Encoding
* StandardScaler
* `predict()` vs `predict_proba()`
* Classification Threshold
* Accuracy
* Precision
* Recall
* Confusion Matrix
* ROC Curve
* AUC
* Coefficients
* Odds Ratio
* Class imbalance

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* Visual Studio Code

## Machine Learning Workflow Practiced

```text
Raw Data
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Feature Encoding
   ↓
Feature Scaling
   ↓
Training / Testing Data
   ↓
Model Training
   ↓
Prediction
   ↓
Model Evaluation
   ↓
Model Interpretation
```

## Internship Progress

Completed:

* Level 1 – Data Preprocessing
* Level 1 – Linear Regression
* Level 2 – Logistic Regression

Further machine learning tasks will be added as the internship progresses.

## Author

**Mostafa Elshafey**

Machine Learning Intern
Codveda Technologies
