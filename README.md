# Term Deposit Subscription Prediction (Bank Marketing ML)

## Project Title
Predicting whether a bank customer will subscribe to a term deposit using marketing and customer data.

---

## Problem Statement
Banks run phone marketing campaigns to promote term deposit products, but most customers do not subscribe.  
Calling every customer is inefficient and costly.

**Objective:**  
Build a machine learning model that predicts whether a customer will subscribe (yes/no) so the bank can prioritize high-probability customers and improve campaign efficiency.

**Dataset:**
- Bank marketing dataset
- ~40,000 customer records
- Demographics, financial status, and campaign information
- Target variable: `y` (yes / no)
- Highly imbalanced (≈7% positive class)

---

## Approach & Methodology

### Data Preparation
- Removed `duration` to prevent data leakage
- Encoded categorical variables using one-hot encoding
- Performed stratified train/test split
- Addressed class imbalance using SMOTE

### Modeling
- Logistic Regression  
- Decision Tree  
- Random Forest  

### Evaluation
- 5-fold cross-validation
- Accuracy (primary metric)
- Recall, F1-score, ROC-AUC
- Confusion matrix

---

## Key Results

| Metric | Result |
|------|------|
| Cross-validated Accuracy | **94.6%** |
| Evaluation Method | 5-fold Cross-Validation |
| Class Imbalance | ~7% “Yes” |

> Note: Due to class imbalance, accuracy alone does not fully capture performance on customers who actually subscribe. Recall and F1-score were also analyzed.

---

## Key Insights
- Most customers do not subscribe; targeting is critical
- Subscription likelihood is influenced by:
  - Age
  - Job type
  - Account balance
  - Loan and housing status
- The model supports customer prioritization rather than blanket calling

---

## Technologies Used
- Python
- pandas, NumPy
- scikit-learn
- imbalanced-learn
- matplotlib, seaborn

---

## How to Run

```bash
git clone https://github.com/your-username/term-deposit-subscription-prediction.git
cd term-deposit-subscription-prediction
pip install -r requirements.txt
jupyter notebook Term_Deposit_Prediction.ipynb

---

## 🛠️ Tools & Technologies
- Python
- pandas, NumPy
- scikit-learn
- imbalanced-learn
- matplotlib, seaborn

---

## 🚀 How to Run the Project
1. Clone the repository  
