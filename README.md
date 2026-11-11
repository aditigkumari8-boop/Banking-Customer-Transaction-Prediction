# Banking Customer Transaction Prediction

## Project Overview

This project focuses on predicting whether a customer will make a transaction using machine learning classification techniques.

The objective is to analyze anonymized banking customer data, identify meaningful patterns, and build predictive models that classify customers into two categories: transaction and no transaction.

## Problem Statement

Financial institutions work with large volumes of customer data. Machine learning can help analyze customer behaviour and identify patterns associated with transaction activity.

This project explores supervised machine learning algorithms to predict the target variable based on customer-related features.

## Project Objectives

- Perform exploratory data analysis (EDA).
- Understand the distribution of transaction and non-transaction classes.
- Identify patterns and relationships among features.
- Prepare data for machine learning.
- Train and compare multiple classification algorithms.
- Evaluate model performance using appropriate metrics.
- Save the best-performing model for future use.

## Dataset Description

The dataset contains:
- `ID_code`: Unique identifier for each record.
- `target`: Binary target variable (0 or 1).
- `var_0` to `var_199`: Anonymized numerical input features.

**Note:** The original dataset is not included in this repository because of its large file size. Place the authorized dataset inside the `Data` folder before running the notebook.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Joblib
- Jupyter Notebook

## Project Workflow

### 1. Data Loading and Understanding
- Imported the dataset using Pandas.
- Examined dataset dimensions, columns, data types and statistical summaries.
- Checked for missing values and duplicate records.

### 2. Exploratory Data Analysis
- Analyzed target class distribution.
- Visualized numerical feature distributions using histograms.
- Identified potential outliers using boxplots.
- Examined feature correlations using heatmaps.

### 3. Data Preprocessing
- Separated independent and dependent variables.
- Removed the unique identifier from model inputs.
- Split the data into training and testing sets.
- Applied feature scaling where required.

### 4. Model Building

Three classification algorithms were implemented:

**Logistic Regression**
- Used as a baseline classification model.
- Applied class weighting to address class imbalance.

**Random Forest**
- Used an ensemble of decision trees.
- Applied balanced class weights.

**XGBoost**
- Implemented gradient boosting for classification.
- Used class weighting to handle class imbalance.

### 5. Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Average Precision
- Confusion Matrix

ROC curves and metric comparison visualizations were also generated.

### 6. Feature Importance

Feature importance analysis was performed using the XGBoost model to identify features contributing most to its predictions.

### 7. Model Saving

The selected model was saved using Joblib in a `.pkl` file for future use.

## Repository Structure

```text
Banking-Customer-Transaction-Prediction/
│
├── Data/
│   └── train(1).csv
│
├── Customer_Transaction_Prediction.ipynb
├── best_customer_transaction_model.pkl
├── .gitignore
└── README.md
```

*The Data folder is kept locally and is not uploaded to this repository.*

## How to Run the Project

1. Clone this repository:

```bash
git clone https://github.com/aditigkumari8-boop/Banking-Customer-Transaction-Prediction.git
```

2. Navigate to the project directory:

```bash
cd Banking-Customer-Transaction-Prediction
```

3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib jupyter
```

4. Place the authorized dataset inside the `Data` folder.

5. Open the Jupyter Notebook:

```bash
jupyter notebook
```

6. Run the notebook cells sequentially.

## Key Learning Outcomes

- Practical understanding of supervised machine learning.
- Data preprocessing and exploratory data analysis.
- Handling imbalanced classification problems.
- Training and comparing multiple ML models.
- Evaluating classification performance.
- Saving and loading trained machine learning models.

## Author

**Aditi Kumari**

- GitHub: https://github.com/aditigkumari8-boop

---

*This project was developed as part of a practical machine learning project to strengthen skills in data analysis and predictive modelling.*
