## COVID-19 Mortality Prediction Using AI

---

## Problem Statement
The COVID-19 pandemic created an urgent need for early identification of high-risk patients. Manual clinical assessment alone may not efficiently predict severe outcomes. This project applies machine learning techniques to analyze patient medical data and predict mortality risk, supporting data-driven healthcare decision-making.

---

## Objective
- Analyze COVID-19 patient clinical and demographic data
- Build a machine learning model to predict patient mortality
- Identify key factors contributing to severe outcomes
- Demonstrate the application of AI in healthcare analytics

---

## Dataset Description
The dataset consists of anonymized COVID-19 patient medical records. Each row represents an individual patient and includes demographic details, medical conditions, treatment indicators, and COVID-19 classification.

### Key Features
- Demographics: Age, Sex, Pregnancy status
- Medical Conditions: Diabetes, Pneumonia, Asthma, Hypertension, Obesity, Renal disease, etc.
- Treatment Information: ICU admission, Intubation
- Target Variable: Patient death status (derived from `DATE_DIED`)

Invalid values (97, 98, 99) are handled during preprocessing.

---

## Methodology / Approach
1. Import dataset using Kaggle API in Google Colab
2. Perform data cleaning and preprocessing
3. Convert patient outcome into binary classification (Death / Survival)
4. Handle missing and invalid values
5. Split data into training and testing sets
6. Train a Random Forest classification model
7. Evaluate model performance using standard metrics
8. Predict mortality risk for new patient data

---

## Tools & Technologies Used
- **Language:** Python
- **Platform:** Google Colab
- **Libraries:**
  - Pandas, NumPy
  - Scikit-learn
- **Dataset Source:** Kaggle

---

## Steps to Run the Project
1. Open Google Colab
2. Upload `kaggle.json` (Kaggle API key)
3. Download the dataset using Kaggle API
4. Load the dataset using Pandas
5. Run preprocessing steps
6. Train the machine learning model
7. Evaluate performance
8. Perform predictions on new patient data

---

## Results / Output
- The model predicts COVID-19 patient mortality with high accuracy
- Age, pneumonia, ICU admission, and comorbidities significantly influence outcomes
- The system provides both class-based and probability-based predictions
- Demonstrates effective use of machine learning for healthcare analysis

---

## Dataset
Dataset used in this project is available on Kaggle:  
https://www.kaggle.com/datasets/meirnizri/covid19-dataset


---

## Future Enhancements
- Use advanced models such as XGBoost
- Add explainable AI (SHAP) for feature importance
- Deploy as a web application
- Extend to predict ICU requirement or severity level

---
