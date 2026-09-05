# Codveda Machine Learning Internship

This repository contains the projects and tasks I completed during my **Machine Learning Internship at Codveda Technologies**.

Throughout the internship, I worked on different machine learning problems covering data preprocessing, regression, classification, ensemble learning, model evaluation, cross-validation, and hyperparameter tuning.

The internship was a valuable hands-on experience that helped me strengthen my understanding of the complete Machine Learning workflow, from preparing raw data to training, evaluating, and improving machine learning models.

---

## Internship Tasks

I completed six tasks across three levels:

### Level 1 - Basic

- Task 1: Data Preprocessing
- Task 2: Linear Regression

### Level 2 - Intermediate

- Task 1: Logistic Regression
- Task 2: Decision Tree Classification

### Level 3 - Advanced

- Task 1: Random Forest Classification
- Task 2: Support Vector Machine (SVM)

---

# Level 1

## Task 1 - Data Preprocessing

### Dataset
Stock Prices Dataset

### Objective
Prepare raw stock market data for machine learning by cleaning, encoding, splitting, and scaling the dataset.

### Work Completed

- Loaded and explored the dataset using Pandas
- Checked dataset shape, data types, and missing values
- Identified rows containing missing values
- Removed a very small number of incomplete rows
- Converted the date column into useful numerical features
- Encoded the stock symbol categorical feature
- Split the dataset into training and testing sets
- Applied StandardScaler to numerical features
- Prevented data leakage by fitting the scaler only on the training data

### Concepts Learned

- Missing value handling
- Data cleaning
- Categorical encoding
- Feature engineering
- Train/Test Split
- Feature Scaling
- Standardization
- Data Leakage

---

## Task 2 - Linear Regression

### Dataset
House Prediction Dataset

### Objective
Build a Linear Regression model to predict continuous house values.

### Work Completed

- Loaded and explored the housing dataset
- Separated features and target variable
- Split the data into training and testing sets
- Trained a Linear Regression model
- Generated predictions on unseen test data
- Evaluated the model using:
  - Mean Squared Error (MSE)
  - R² Score
- Analyzed model coefficients and intercept
- Visualized Actual vs Predicted values

### Concepts Learned

- Regression
- Continuous target prediction
- Features and target variables
- Model training and prediction
- Mean Squared Error
- R² Score
- Linear model coefficients
- Model evaluation

---

# Level 2

## Task 1 - Logistic Regression

### Dataset
Customer Churn Dataset

### Objective
Predict whether a customer will churn using Logistic Regression.

### Work Completed

- Loaded separate training and testing churn datasets
- Prepared features and target variable
- Converted the churn target into binary values
- Applied One-Hot Encoding to categorical features
- Scaled numerical features using StandardScaler
- Trained a Logistic Regression classifier
- Generated class predictions and churn probabilities
- Evaluated the model using:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Confusion Matrix
  - Classification Report
  - ROC Curve
  - AUC Score
- Investigated classification threshold effects
- Analyzed model coefficients and odds ratios
- Studied the impact of class imbalance

### Model Results

| Metric | Score |
|---|---:|
| Accuracy | 85.46% |
| Precision | 47.73% |
| Recall | 22.11% |
| AUC | 81.38% |

### Key Observation

Although the model achieved approximately 85% accuracy, the dataset was imbalanced. Therefore, accuracy alone was not sufficient to evaluate the classifier.

The ROC-AUC score showed that the model had reasonable class-separation ability, while the relatively low recall indicated that many churn customers were not detected at the default classification threshold.

### Concepts Learned

- Binary Classification
- Logistic Regression
- Probability Prediction
- Classification Thresholds
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC Curve
- AUC
- Class Imbalance
- Odds Ratios

---

## Task 2 - Decision Tree Classification

### Dataset
Iris Dataset

### Objective
Classify Iris flower species using a Decision Tree and investigate overfitting and pruning.

### Work Completed

- Loaded and explored the Iris dataset
- Separated the input features and species target
- Used stratified Train/Test splitting
- Trained an unrestricted Decision Tree
- Evaluated the original model
- Visualized the Decision Tree
- Analyzed Gini impurity, nodes, branches, and leaves
- Compared training and testing accuracy
- Applied pre-pruning using `max_depth`
- Evaluated the pruned model
- Analyzed feature importance

### Model Results

| Model | Train Accuracy | Test Accuracy | F1 Score |
|---|---:|---:|---:|
| Original Decision Tree | 100.00% | 93.33% | 93.33% |
| Pruned Decision Tree | 98.33% | 96.67% | 96.66% |

### Key Observation

The original tree achieved perfect training accuracy but lower testing accuracy, indicating slight overfitting.

After limiting the tree depth, training accuracy decreased slightly while testing accuracy and F1-score improved.

This demonstrated how controlling model complexity can improve generalization.

### Concepts Learned

- Decision Trees
- Root Nodes
- Splits
- Branches
- Leaf Nodes
- Gini Impurity
- Feature Importance
- Overfitting
- Pre-Pruning
- Model Complexity
- Generalization

---

# Level 3

## Task 1 - Random Forest Classification

### Dataset
Iris Dataset

### Objective
Use an ensemble of Decision Trees to classify Iris flower species and optimize the model using Cross-Validation and Hyperparameter Tuning.

### Work Completed

- Built a baseline Random Forest classifier
- Used multiple Decision Trees for ensemble prediction
- Evaluated the model using:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Confusion Matrix
  - Classification Report
- Analyzed feature importance
- Applied 5-Fold Cross-Validation
- Tuned Random Forest hyperparameters using GridSearchCV
- Tested different values for:
  - `n_estimators`
  - `max_depth`
  - `min_samples_split`
  - `min_samples_leaf`
- Compared the baseline and tuned models

### Concepts Learned

- Ensemble Learning
- Random Forest
- Bootstrap Sampling
- Random Feature Selection
- Majority Voting
- Cross-Validation
- Hyperparameters
- GridSearchCV
- Model Selection
- Feature Importance
- Generalization

### Results

Add your final Random Forest results here:

| Metric | Baseline Model | Tuned Model |
|---|---:|---:|
| Accuracy | XX% | XX% |
| Precision | XX% | XX% |
| Recall | XX% | XX% |
| F1-Score | XX% | XX% |

---

## Task 2 - Support Vector Machine (SVM)

### Dataset
Iris Dataset

### Objective
Classify Iris species using Support Vector Machine and optimize the decision boundary using different kernels and hyperparameters.

### Work Completed

- Split the dataset using stratified Train/Test splitting
- Applied StandardScaler
- Trained a baseline SVM classifier
- Evaluated the model using:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Confusion Matrix
  - Classification Report
- Investigated Support Vectors and Margin
- Compared different kernels:
  - Linear
  - RBF
  - Polynomial
  - Sigmoid
- Applied Cross-Validation
- Created a Scikit-learn Pipeline
- Used GridSearchCV for Hyperparameter Tuning
- Tuned:
  - `C`
  - `gamma`
  - `kernel`
- Prevented data leakage by including StandardScaler inside the Pipeline
- Compared baseline and tuned SVM models

### Concepts Learned

- Support Vector Machine
- Decision Boundary
- Hyperplane
- Margin
- Support Vectors
- Linear and Non-Linear Classification
- Kernel Trick
- RBF Kernel
- C Hyperparameter
- Gamma Hyperparameter
- Feature Scaling
- Pipeline
- Cross-Validation
- GridSearchCV
- Data Leakage Prevention

### Results

Add your final SVM results here:

| Metric | Baseline Model | Tuned Model |
|---|---:|---:|
| Accuracy | XX% | XX% |
| Precision | XX% | XX% |
| Recall | XX% | XX% |
| F1-Score | XX% | XX% |

---

# Machine Learning Workflow

Across the internship projects, I followed the general Machine Learning workflow:

```text
Raw Data
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Feature Engineering
   ↓
Categorical Encoding
   ↓
Feature Scaling (when required)
   ↓
Train/Test Split
   ↓
Model Training
   ↓
Prediction
   ↓
Model Evaluation
   ↓
Cross-Validation
   ↓
Hyperparameter Tuning
   ↓
Final Model Evaluation
```

---

# Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Visual Studio Code
- Git
- GitHub

---

# Machine Learning Algorithms Implemented

During the internship, I implemented and studied:

- Linear Regression
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine

I also gained practical experience with data preprocessing, feature engineering, model evaluation, cross-validation, hyperparameter tuning, and ensemble learning.

---

# Important Concepts Learned

Some of the most important Machine Learning concepts I practiced during this internship include:

- Supervised Learning
- Regression
- Binary Classification
- Multiclass Classification
- Train/Test Splitting
- Feature Scaling
- One-Hot Encoding
- Label Encoding
- Data Leakage
- Overfitting
- Generalization
- Precision and Recall
- F1-Score
- Confusion Matrix
- ROC-AUC
- Feature Importance
- Decision Tree Pruning
- Ensemble Learning
- Cross-Validation
- Hyperparameter Tuning
- GridSearchCV
- Machine Learning Pipelines

---

# Project Structure

```text
Codveda-Machine-Learning/
│
├── level_1/
│   │
│   ├── task_1_data_preprocessing/
│   │   ├── dataset/
│   │   └── task_1_data_preprocessing.ipynb
│   │
│   └── task_2_linear_regression/
│       ├── dataset/
│       └── task_2_linear_regression.ipynb
│
├── level_2/
│   │
│   ├── task_1_logistic_regression/
│   │   ├── dataset/
│   │   └── task_1_logistic_regression.ipynb
│   │
│   └── task_2_decision_tree/
│       ├── dataset/
│       └── task_2_decision_tree.ipynb
│
├── level_3/
│   │
│   ├── task_1_random_forest/
│   │   ├── dataset/
│   │   └── task_1_random_forest.ipynb
│   │
│   └── task_2_svm/
│       ├── dataset/
│       └── task_2_svm.ipynb
│
└── README.md
```

---

# How to Run the Projects

1. Clone the repository.

```bash
git clone https://github.com/mostafaelshafey27/Codveda-Machine-Learning.git
```

2. Install the required Python libraries.

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

3. Open the project using VS Code or Jupyter Notebook.

4. Navigate to the required task folder.

5. Run the notebook cells sequentially.

---

# Internship Experience

This internship helped me move beyond simply implementing machine learning algorithms and develop a better understanding of why each step in the Machine Learning pipeline is important.

I gained practical experience in preparing datasets, selecting suitable models, evaluating their performance, identifying problems such as overfitting and class imbalance, and improving models using Cross-Validation and Hyperparameter Tuning.

One of the most valuable aspects of the internship was learning how different algorithms behave and when each model may be appropriate for a particular problem.

I am grateful to **Codveda Technologies** for providing this opportunity and for the practical learning experience throughout the internship.

---

# Author

**Mostafa Elshafey**

Machine Learning Intern  
Codveda Technologies

GitHub:  
https://github.com/mostafaelshafey27

---

## Repository

Codveda Machine Learning Internship:

https://github.com/mostafaelshafey27/Codveda-Machine-Learning