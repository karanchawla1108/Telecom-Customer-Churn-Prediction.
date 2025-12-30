# Telecom Customer Churn Prediction – Data Analytics Project

This project focuses on predicting customer churn in the telecommunications sector using data analytics and machine learning techniques.  Churn is when a telecommunications customer no longer utilizes the service, thus impacting the profitability of the business. Here, the focus is finding such at-risk telecommunications customers and providing data-driven insights to retain them.

This project is conducted within the COM6035M Data Analytics module offered by York St John University.
## Objectives
- Analyze customer behavior for data points contributing to customer churn
- Deal with real-world concerns such as missing values and imbalanced classes
- Developing and testing machine learning models for the prediction of churn

- Compare the performance of the models using the correct metrics
- Offering useful business recommendations based on model results
Dataset Description

## Methodology
1. Exploratory Data Analysis (EDA
- Applied histograms and scatter plots to interpret distributions and relationships
- Examined the correlation data for relationships between the variables
- Identified churn patterns from usage, billing, and customer service data
2. Data Preprocessing
- Handled missing values with:

- Median imputation for numbers
- Mode imputation for categorical variables
- Encoded categorical variables

- Scaled features with StandardScaler </s>
- Handled class imbalance problem by applying SMOTE (Synthetic Minority Over-sampling Technique)
3. Feature Engineering &amp; Selection
- Added only a few explicit features since the data is rather rich
- Scaled and encoded features that facilitate model learning

- Verified feature importance by tree based models

4. Model Development
Models used:
- Logistic Regression (Baseline)
- Random Forest
- Gradient Boosting
- XGBoost
To improve the performance, hyperparameter tuning was used for ensemble models.
5. Model evaluation

• Employed 10-fold cross-validation for establishing robust estimates
- Metrics:
- Accuracy
- Precision

- Recall
- F1_SCORE
- ROC-AUC

- Conducted paired t-tests for model performance comparison
Results Summary

## Result Summary
- Logistics Regression offered a simple explanation with a weak recall value for customers who actually churned
- Ensemble methods generally outperformed linear methods

- Tuned XGBoost performed the best, with improvements observed in precision, F1 score, and ROC AUC
Demonstrates that ensemble learning is effective for churn prediction on imbalanced datasets

## Key Insights
- There is a strong link between customer service inquiries and customer churn
- Unreliable billing, such as dropping usage, is a critical churn signal
- Newly acquired customers are prone to churn

## Business Recommendations
- Contact customers displaying early signs of churn
- Provide added support to customers who frequently request help
- Provide flexible packages for budget-sensitive consumers
- Monitor for any decline in use to trigger the retention mechanism

## Technologies Used
- Python
- pandas, NumPy
- matplotlib, seaborn

- Scikit-
- Imbalanced-Learn (SMOTE)
- XGBoost
- Jupyter Notebook

## Repository Structure


```
  |--cell2celltrain_Small_6k (Raw Data)
  |
  |--Readme (Project Description)
  |
  |--Requirement.txt (Require download tools)
  |
  |--model_training.ipynb (Trained Model)
  |
  |--Untitled (Rough try to train another model on the basic of train model)
  |
  |--xgb.pkl (Saved Trained Model)

```

## How to Run

  Clone the repository
 
### Jupyter Notebook
   1. Install the classic Jupyter Notebook with:
   ```
   pip install notebook
   ```
   2. To run the notebook:
   ```
   jupyter notebook
   ```
   3. Install dependencies using:
   ```
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook and run cells sequentially

---

## Ethical Issues 

Anonymized data is used throughout. This churn predictor is a tool that can help improve service quality, not make discriminatory predictions. 

## Author

Karan Chawla

BSc (Hons) Computer Science
York St John University

---

## Disclaimer

This project was completed for academic purposes as part of a university assessment. The findings should not be considered as production-ready without further validation and testing.