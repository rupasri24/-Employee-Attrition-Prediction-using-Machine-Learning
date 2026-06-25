# Employee Attrition Prediction using Machine Learning

## Project Overview

This project predicts whether an employee is likely to leave the company using HR-related features such as job satisfaction, monthly income, overtime, work-life balance, years at company, and job role. The objective is to help HR teams identify employees at higher risk of attrition and take proactive retention actions.

## Dataset

* **Dataset Name:** IBM HR Analytics Employee Attrition Dataset
* **Source:** Kaggle
* **File Used:** `HR_Attrition.csv`

## Tools & Libraries Used

* Python
* Google Colab / Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

## Project Workflow

1. **Data Loading and Exploration**

   * Loaded the HR attrition dataset
   * Checked dataset shape, data types, and target variable distribution
   * Calculated attrition rate and identified numeric and categorical columns

2. **Data Cleaning and Preprocessing**

   * Checked for missing values
   * Dropped irrelevant columns such as `EmployeeNumber`, `Over18`, `StandardHours`, and `EmployeeCount`
   * Converted the target column `Attrition` from Yes/No to 1/0
   * Applied one-hot encoding to categorical variables
   * Scaled numeric features using `StandardScaler`

3. **Exploratory Data Analysis (EDA)**

   * Analyzed attrition rate by department and job role
   * Compared monthly income of employees who stayed vs left
   * Studied attrition patterns by work-life balance and years at company
   * Identified key business insights from the data

4. **Model Building and Comparison**

   * Split data into training and test sets
   * Trained three classification models:

     * Logistic Regression
     * Random Forest Classifier
     * Gradient Boosting Classifier

5. **Model Evaluation**

   * Evaluated models using:

     * Precision
     * Recall
     * F1-Score
     * ROC-AUC Score
     * Confusion Matrix
   * Selected the best-performing model
   * Extracted top feature importances

6. **Visualization**

   * Attrition rate by department
   * Attrition rate by job role
   * Monthly income vs attrition
   * Confusion matrix heatmap
   * Top 10 feature importances
   * ROC curve comparison of models

7. **HR Insights and Recommendations**

   * Identified the strongest factors driving employee attrition
   * Highlighted high-risk departments / job roles
   * Suggested business recommendations for employee retention

## Machine Learning Models Used

* Logistic Regression
* Random Forest Classifier
* Gradient Boosting Classifier

## Evaluation Metrics

* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix

## Project Files

* `analysis.ipynb` — Complete notebook with code and analysis
* `HR_Attrition.csv` — Dataset used for the project
* `summary.docx` / `summary.pdf` — 1-page HR-friendly summary
* `charts/` — Saved visualization images

## Business Goal

The purpose of this project is not only to predict employee attrition, but also to identify the key factors driving attrition so that HR teams can improve employee retention and reduce turnover costs.

## How to Run

1. Open `analysis.ipynb` in Google Colab or Jupyter Notebook
2. Upload `HR_Attrition.csv`
3. Run all cells from top to bottom
4. Review the model comparison table, charts, and HR insights section

## Future Improvements

* Hyperparameter tuning for better model performance
* Use SMOTE or other balancing techniques for class imbalance
* Deploy the model using Flask or Streamlit
* Add dashboard-based HR reporting for easier business use
