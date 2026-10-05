# Decision Tree Classifier - Bank Marketing Dataset

## Project Overview

This project uses a Decision Tree Classifier to predict whether a customer will subscribe to a term deposit based on information from a bank marketing campaign.

The project was completed as part of the ArithMatrix Virtual Internship Program 2026 in the Data Science domain.

## Dataset

The project uses the Bank Marketing Dataset from the UCI Machine Learning Repository.

Dataset Source:
https://archive.ics.uci.edu/ml/datasets/bank+marketing

The dataset contains information about customers contacted during marketing campaigns.

### Target Variable

The target variable is `y`.

- `yes` - Customer subscribed to a term deposit
- `no` - Customer did not subscribe to a term deposit

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the Bank Marketing dataset.
2. Separated the features and target variable.
3. Converted the target values from `no/yes` to `0/1`.
4. Identified numerical and categorical features.
5. Applied One-Hot Encoding to categorical features.
6. Kept numerical features unchanged.
7. Split the dataset into 80% training data and 20% testing data.
8. Used stratified splitting to maintain the target class distribution.

## Model

A Decision Tree Classifier was trained using Scikit-learn.

The model was configured with:

- Maximum depth: 5
- Class weight: Balanced
- Random state: 42

## Model Evaluation

The model was evaluated using the test dataset.

### Results

- Accuracy: 75.56%
- Precision: 30.67%
- Recall: 86.39%

### Confusion Matrix

The confusion matrix was generated and saved as:

`confusion_matrix.png`

### Top 5 Important Features

| Rank | Feature | Importance |
|---|---|---:|
| 1 | duration | 0.5810 |
| 2 | poutcome | 0.1831 |
| 3 | contact | 0.1186 |
| 4 | housing | 0.0766 |
| 5 | month | 0.0369 |

The feature importance chart was saved as:

`top_5_feature_importance.png`

## Key Findings

- `duration` was the most important feature used by the Decision Tree.
- Previous campaign outcome (`poutcome`) was the second most important feature.
- Contact type, housing loan status, and month also contributed to the model's predictions.
- The model achieved a recall of 86.39%, meaning it identified a large proportion of customers who actually subscribed.

## Conclusion

The Decision Tree Classifier was successfully implemented for predicting customer subscription to a term deposit. The project demonstrates data preprocessing, categorical feature encoding, model training, prediction, evaluation, confusion matrix analysis, and feature importance analysis.

## Project Files

- `Decision_Tree_Classifier.ipynb` - Jupyter Notebook containing the complete analysis and model
- `confusion_matrix.png` - Confusion matrix visualization
- `top_5_feature_importance.png` - Top 5 feature importance visualization
- `README.md` - Project documentation

## How to Run

1. Install Python.
2. Install the required libraries.
3. Open the Jupyter Notebook.
4. Run the cells from top to bottom.

The notebook downloads the dataset directly from the UCI Machine Learning Repository.