# Telco Customer Churn Prediction

This project analyzes customer churn behavior in a telecom company using Python and machine learning.  
It includes a complete pipeline from data cleaning to model training, evaluation, and business insights.  
A separate Tableau dashboard presents the findings visually.

## 📂 Files in This Repository

- `Telco_Churn_Prediction.ipynb` – full Google Colab notebook with code and results  
- `requirements.txt` – Python dependencies for running the code  
- `README.md` – project summary and instructions

# This is my first Tableau dashboard. I'm continuously learning and will improve with each project
 
- Tableau dashboard: (https://public.tableau.com/app/profile/shruti.s5837/viz/Book1_17531819643920/Dashboard1) 

---

## 📊 Business Problem

Telecom companies often lose customers due to various service or pricing issues.  
This project aims to **predict whether a customer will churn**, using historical customer data, and uncover the key drivers behind churn.

---

## 📁 Dataset

- **Name**: Telco Customer Churn  
- **Source**: [Kaggle Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)  
- **Records**: 7,043 customer entries  
- **Target Variable**: `Churn` (Yes/No)

---

## 🛠 Tools & Libraries

- Python  
- pandas, numpy  
- scikit-learn  
- matplotlib (optional, not used here)  
- Google Colab

---

## ⚙️ Machine Learning Model

### Model Used:
- **Logistic Regression** (with feature scaling using `StandardScaler`)

### Preprocessing Steps:
- Dropped customer IDs
- Converted `TotalCharges` to numeric
- Handled missing values
- One-hot encoded categorical variables
- Scaled features using `StandardScaler`

---

## Model Evaluation

- **Accuracy**: ~79.5%  
- **Classification Report**:
  - Precision, recall, F1-score for churn vs non-churn
- **Confusion Matrix**: Included in the output

---

## 🔍 Feature Importance

Top 10 most influential features by absolute coefficient value:

| Feature                     | Influence |
|----------------------------|-----------|
| `tenure`                   | High      |
| `TotalCharges`             | Moderate  |
| `MonthlyCharges`           | Moderate  |
| `InternetService_Fiber optic` | Moderate |
| `Contract_Month-to-month`  | Moderate  |
| `Contract_Two year`        | Moderate  |
| `InternetService_DSL`      | Moderate  |
| `StreamingTV_Yes`          | Low       |
| `StreamingMovies_Yes`      | Low       |
| `OnlineSecurity_No`        | Low       |

---

## 📈 Tableau Dashboard

An interactive dashboard was built using Tableau to visualize:
- Churn rate (pie chart)
- Average monthly charges by churn status
- Churn by contract type
- Tenure distribution histogram

**Dashboard Link**: (https://public.tableau.com/app/profile/shruti.s5837/viz/Book1_17531819643920/Dashboard1)  

