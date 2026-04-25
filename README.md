# Loan Risk Analysis

This repository contains a kaggle Notebook (`loan-risk-anlysis-2.ipynb`) that performs a comprehensive risk analysis on loan applications to predict whether a loan will be approved or rejected.

## Project Overview

The main objective of this project is to build machine learning models to automate the loan eligibility process based on customer details provided while filling out an online application form. These details include Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History, and others.

## Notebook Contents

The `loan-risk-anlysis-2 (1).ipynb` notebook covers the following steps:

1. **Data Loading & Exploration:**
   - Loading the dataset using pandas.
   - Initial exploration to understand the data's shape, features, and the distribution of the target variable (`Loan_Status`).

2. **Data Cleaning & Preprocessing:**
   - Handling missing values: filling numerical missing values with the median and categorical missing values with the mode.
   - Encoding categorical variables into a numerical format suitable for machine learning algorithms using `LabelEncoder`.

3. **Feature Engineering:**
   - Creating new features such as `TotalIncome` by combining `ApplicantIncome` and `CoapplicantIncome` to capture the overall financial capability of the applicant.
   - Dropping unnecessary identifiers like `Loan_ID`.

4. **Exploratory Data Analysis (EDA) & Visualization:**
   - Visualizing the distribution of loan approvals.
   - Analyzing the relationship between `TotalIncome` and `Loan_Status`.
   - Generating a correlation heatmap to identify the most significant features (e.g., `Credit_History` has a strong correlation with loan approval).

5. **Model Building & Evaluation:**
   - Splitting the data into training and testing sets.
   - Training classification models (e.g., Random Forest Classifier, Logistic Regression).
   - Evaluating model performance using metrics such as Accuracy, Precision, Recall, F1-Score, and ROC-AUC.

## Dependencies

To run the notebook, you will need the following Python libraries installed:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

You can install these dependencies using `pip`:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run

1. Ensure you have Jupyter Notebook or use kaggle installed.
2. Clone or download this repository.
3. Open a terminal or command prompt and navigate to the directory containing the notebook.
4. Run `jupyter notebook` to start the Jupyter interface.
5. Open `loan-risk-anlysis-2 (1).ipynb` and execute the cells sequentially. Make sure to update the dataset path in the first code cell to point to your local copy of the dataset.

## Dataset

The analysis uses a loan prediction dataset containing various applicant attributes. Ensure the dataset (`train_u6lujuX_CVtuZ9i.csv` or similar) is available in your environment before running the notebook.


contributors:
AbramMaged

