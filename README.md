# 📊 Data Pipeline & Model Validation for Credit Risk Prediction

## 📌 Project Overview
This project implements an **end-to-end data pipeline and model validation workflow** for credit risk prediction using structured financial data. The objective is to ensure **data reliability, validation, and reproducibility** before deploying a machine learning model in a real-world business environment.

The project simulates how data and risk analytics teams validate datasets and models before using them for **credit decisioning**.

---

## 🎯 Business Objective
To predict the likelihood of customer default while ensuring:
- High data quality and integrity  
- Compliance with business validation rules  
- Reliable and interpretable model performance  

---

## 🛠️ Technology Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Joblib  
- **Environment:** Google Colab  
- **Storage:** Google Drive  
- **Version Control:** GitHub  

---

## 📂 Project Structure
data-pipeline-model-validation/
│
├── data/
│ ├── raw/
│ │ └── credit_data.csv
│ └── processed/
│ └── clean_credit_data.csv
│
├── notebooks/
│ └── data_pipeline_model_validation.ipynb
│
├── models/
│ └── credit_risk_model.pkl
│
├── reports/
│ └── model_evaluation.txt
│
└── README.md

---

## 🔄 Project Workflow

### 1️⃣ Data Ingestion
- Loaded raw credit data from storage
- Verified schema, data types, and column consistency

### 2️⃣ Data Quality Checks
- Checked missing values, duplicates, and invalid entries
- Identified unrealistic and undefined categorical values

### 3️⃣ Data Cleaning & Preparation
- Handled invalid values in age and categorical fields
- Applied appropriate imputation techniques
- Generated a clean, analysis-ready dataset

### 4️⃣ Data Validation Rules
- Applied business rules such as:
  - Valid age range
  - Non-negative financial values
  - Domain constraints for categorical variables

### 5️⃣ Model Training
- Trained a Logistic Regression model for default prediction
- Used stratified train-test split to handle class imbalance

### 6️⃣ Model Validation
- Evaluated model using accuracy, precision, recall, and F1-score
- Analyzed misclassification impact from a business perspective

### 7️⃣ Model Persistence
- Saved trained model using `joblib`
- Stored model artifact for reuse and deployment readiness

---

## 📈 Model Performance Summary
Key evaluation metrics are documented in: reports/model_evaluation.txt
This includes classification metrics used to validate model reliability.

---

## 💾 Saved Artifacts
- **Processed Data:** `data/processed/clean_credit_data.csv`
- **Trained Model:** `models/credit_risk_model.pkl`
- **Evaluation Report:** `reports/model_evaluation.txt`

---

## 📌 Key Learnings
- Importance of data validation before modeling
- Building reproducible and auditable data pipelines
- Applying business rules to analytical workflows
- Model evaluation and persistence best practices

---

## 🚀 Future Enhancements
- Implement cross-validation and hyperparameter tuning
- Automate pipeline using sklearn Pipelines
- Deploy model using Flask or FastAPI
- Monitor data drift and model performance

---

## 👩‍💻 Author
**Shreya Itkapalle**  
Aspiring Data Analyst / Data Scientist  

---
