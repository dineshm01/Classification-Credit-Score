# Credit Score Classification

## Project Overview

This project focuses on building a **Credit Score Classification Model** to categorize customers into different credit score groups (`Poor`, `Standard`, `Good`) based on financial and personal attributes. The dataset was preprocessed, cleaned, and multiple machine learning models were applied and evaluated.

## Dataset

* **File:** `credit_score.csv.gz(Zip File)`
* The dataset contains customer details such as income, occupation, outstanding debt, payment behavior, number of loans, delayed payments, and other financial information.
* Target variable: **Credit\_Score** (`Poor`, `Standard`, `Good`)

## Data Preprocessing

1. Dropped irrelevant columns (`ID`, `Customer_ID`, `Name`, `SSN`, etc.).
2. Handled missing values using **forward fill** and **backward fill**.
3. Cleaned categorical placeholders like `"______"`, `"!@9#%8"`, `"NM"`.
4. Converted categorical values into numerical form using **Label Encoding**.
5. Replaced outliers using **IQR filtering**.
6. Standardized features using **StandardScaler**.

## Machine Learning Models Used

* **Logistic Regression**
* **Decision Tree Classifier**

  * Hyperparameter tuning with **GridSearchCV**
* **Random Forest Classifier**

## Model Evaluation

* Evaluation metric: **Accuracy Score**
* Example results (accuracy may vary):

  * Logistic Regression → \~62%
  * Decision Tree → \~64%
  * Decision Tree (Tuned) → \~67%
  * Random Forest → \~75%

## Tech Stack

* **Python**
* **Pandas, NumPy** → Data manipulation
* **Matplotlib, Seaborn** → Data visualization
* **Scikit-learn** → ML models, preprocessing, evaluation
* **Statsmodels** → Variance Inflation Factor (VIF) analysis

## Results & Insights

* Customers with **higher income** and **good payment behavior** tend to have better credit scores.
* Delayed payments and high outstanding debt negatively impact credit scores.
