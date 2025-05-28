# Home Loan Approval Prediction

An end-to-end machine learning project designed to predict the approval of home loan applications based on demographic and financial data. This project leverages classification models, hyperparameter tuning, and visual analytics to support decision-making in the financial sector.

---

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Data Preprocessing & EDA](#data-preprocessing--eda)
- [Modeling](#modeling)
- [Results](#results)
- [Conclusion](#conclusion)
- [Supplementary Documents](#supplementary-documents)
- [How to Run](#how-to-run)
- [Contact](#contact)

---

## Overview

This project addresses a real-world challenge in automating the loan eligibility process for financial institutions. Using historical data, we built models to assess the likelihood of home loan approval and identify key influencing features like credit history, marital status, and property area.

**Objectives:**
- Analyze factors influencing home loan approval
- Build and evaluate machine learning models
- Visualize insights and model outcomes

---

## Dataset

- **Source:** Dream Housing Finance Company dataset
- **Size:** 600+ records
- **Features Include:**
  - Gender, Marital Status, Dependents, Education, Self-Employed
  - ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Term
  - Credit_History, Property_Area, Loan_Status (target)

📁 [Download Dataset (CSV)](https://github.com/KiruthikaRamadoss/Home-Loan-Approval-Prediction/blob/main/Training%20Dataset.csv)

---

## Data Preprocessing & EDA

- **Missing Values:** Handled 7 columns with missing values; imputed using mean/mode or dropped.
- **Encoding:** Label encoded all categorical columns.
- **EDA Insights:**
  - Higher approval rates for married applicants and those with good credit history.
  - Applicants from semi-urban areas had better approval likelihood.
  - Longer loan terms (e.g., 480 months) had lower approval rates.

📓 [View Jupyter Notebook](HomeLoan.ipynb)

---

## Modeling

- **Train/Test Split:** 80/20
- **Algorithms Used:**
  - Logistic Regression
  - Probit Regression
  - Support Vector Classifier (SVC)
  - Random Forest
  - LightGBM

- **Hyperparameter Tuning:**
  - GridSearchCV and RandomizedSearchCV for Logistic Regression
  - RFE for feature selection

---

## Results

- **Best Model:** Logistic Regression (after tuning)
- **Performance Metrics:**
  - **Accuracy:** 86.48%
  - **Precision:** 85%
  - **Recall:** 99%
  - **ROC AUC:** 0.75
- **Top Influential Features:**
  - Credit_History
  - Property_Area
  - Marital_Status

---

## Conclusion

Logistic Regression (with RandomizedSearchCV) was chosen as the best model due to its interpretability and high performance. It accurately predicted loan approvals and highlighted key features impacting decision-making. The project illustrates how ML models can enhance risk assessment in loan approval pipelines.

---

## Supplementary Documents

📊 [Presentation Slides (PDF)](https://drive.google.com/file/d/100qGDoeCBk1JYxiBzP2iAC0taITXHPOY/view?usp=drive_link)
📄 [Final Report (PDF)](https://drive.google.com/file/d/1AtJYbE3rZxJ_A9UKG4N6Nbgvigol5qxt/view?usp=drive_link)  

*Documents are shared as view-only to protect integrity and prevent unauthorized edits.*

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/YourUsername/HomeLoan-Approval-Prediction.git
   cd HomeLoan-Approval-Prediction
   
2. Create and activate a virtual environment (Optional):
   python -m venv env
   source env/bin/activate  # On Windows use `env\Scripts\activate`

3. Install dependencies:
   pip install -r requirements.txt

4. Launch the notebook:
   jupyter notebook HomeLoan.ipynb

---

## Contact

For inquiries, collaboration, or feedback:

- [LinkedIn](https://www.linkedin.com/in/kiruthikaramadoss/)
- [GitHub](https://github.com/KiruthikaRamadoss)
- [Email](mailto:k_r549@txstate.edu)
  
