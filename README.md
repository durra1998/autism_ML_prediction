# Autism Prediction Using Machine Learning
This project implements a complete machine learning pipeline to predict the likelihood of **Autism Spectrum Disorder (ASD)** using screening and demographic data. The focus is on exploratory data analysis, data preprocessing, model training, hyperparameter tuning, and performance evaluation.

---

## Project Objectives

- Perform **Exploratory Data Analysis (EDA)**
- Preprocess the data using encoding and class balancing
- Train and compare multiple machine learning models
- Apply **hyperparameter tuning** to improve performance
- Evaluate and select the **best-performing model**


---

## Dataset

- The dataset contains demographic details and results from ASD screening questions.
- **Target variable**: Whether the individual is likely to have ASD (1 = yes, 0 = no)
- Dataset source: [UCI Machine Learning Repository – Autism Screening Data](https://archive.ics.uci.edu/ml/datasets/Autism+Screening+Adult)

---

## Workflow Summary

1. **EDA**:
   - Examined class distribution, missing values, and feature types
   - Mapped and cleaned country names and other categorical variables

2. **Preprocessing**:
   - Applied `LabelEncoder` for categorical features  
   - Used **SMOTE** to handle class imbalance

3. **Modeling**:
   - Trained three classifiers:
     - Decision Tree
     - Random Forest
     - XGBoost
   - Performed **5-fold cross-validation**

4. **Hyperparameter Tuning**:
   - Used `RandomizedSearchCV` to find optimal parameters for each model

5. **Model Selection**:
   - Compared best cross-validation accuracy
   - Saved the top model as `best_model.pkl`

6. **Evaluation**:
   - Evaluated the best model on test set using:
     - Accuracy score
     - Confusion matrix
     - Classification report (precision, recall, F1-score)

---



