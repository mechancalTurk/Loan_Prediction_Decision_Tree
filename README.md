# Loan Prediction using a Decision Tree

A machine learning project for predicting loan approval using a Decision Tree classifier implemented in Python with scikit-learn.

The project demonstrates the complete workflow from data preparation and preprocessing to model training, evaluation, visualization, and feature importance analysis.

## Project Overview

The objective of this project is to predict whether a loan application will be approved (`Y`) or rejected (`N`) based on applicant and loan-related characteristics.

A Decision Tree classifier is used because it provides an interpretable model whose decision-making process and feature importance can be examined directly.

## Dataset

The project uses a synthetic loan dataset created specifically for educational and demonstration purposes.

The dataset contains:

- 300 observations
- 13 variables
- Applicant demographic and financial information
- Loan-related information
- Credit history
- Loan approval status (`Loan_Status`)

The target variable contains approximately:

- 66.3% approved loans (`Y`)
- 33.7% rejected loans (`N`)

The dataset does not contain real customer data or personally identifiable information.

## Technologies

- Python
- pandas
- NumPy
- Matplotlib
- scikit-learn
- Jupyter Notebook

## Machine Learning Model

The prediction model is based on:

**DecisionTreeClassifier — scikit-learn**

The dataset is divided into training and test sets, and the trained model is evaluated using several classification metrics.

## Model Evaluation

The Decision Tree achieved the following results:

| Metric | Result |
|---|---:|
| Training Accuracy | 87.6% |
| Test Accuracy | 82.2% |
| Precision | 84.4% |
| Recall | 90.0% |
| F1-Score | 87.1% |
| ROC-AUC | 0.786 |

The moderately higher training accuracy compared with the test accuracy may indicate slight overfitting.

Because the dataset is moderately imbalanced, model performance is not evaluated using accuracy alone. Precision, recall, F1-score, the confusion matrix, and ROC-AUC are also considered.

## Feature Importance

Feature importance analysis is used to examine which variables contributed most strongly to the Decision Tree's predictions.

Credit history is the most important feature, followed by the relationship between applicant income and loan amount.

This provides an additional control check that the model learned meaningful patterns from the synthetic dataset.

## Repository Structure

```text
Loan-Prediction-Decision-Tree/
│
├── README.md
├── Loan_Prediction_Decision_Tree.ipynb
│
├── data/
│   └── loan_dataset_sauber.csv
│
├── images/
│   ├── decision_tree.png
│   ├── confusion_matrix.png
│   └── feature_importance.png
│
├── requirements.txt
└── LICENSE
