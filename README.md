# Term Deposit Subscription Prediction (Bank Marketing ML)

## 📖 Project Overview
Banks often run marketing campaigns to offer customers investment products like term deposits.  
However, calling every customer is expensive and inefficient because most customers say **no**.

This project uses **machine learning** to predict which customers are more likely to subscribe to a term deposit, so banks can focus on the **right customers first**.

---

## 🎯 Project Goal
Predict whether a customer will subscribe (**yes/no**) to a term deposit using marketing and customer data.

---

## 📊 Dataset
- Real-world bank marketing dataset
- 40,000 customer records
- Includes:
  - age, job, education
  - account balance
  - loan and housing status
  - marketing campaign details
- Target variable: `y` (yes / no)

Only **7.24%** of customers subscribed, making this a **highly imbalanced dataset**.

---

## ⚙️ What Was Done

### 1. Data Preparation
- Removed the `duration` column to prevent data leakage
- Converted categorical data into numerical values
- Split data into training and testing sets
- Used SMOTE to balance the dataset

### 2. Modeling
Trained and compared multiple models:
- Logistic Regression
- Decision Tree
- Random Forest

### 3. Evaluation
- Used **5-fold cross-validation**
- Evaluated using:
  - Accuracy
  - Recall
  - F1-score
  - ROC-AUC
  - Confusion Matrix

---

## ✅ Results
- Achieved **94.6% average accuracy** using 5-fold cross-validation  
- Exceeded the required **81% accuracy** threshold
- Identified key features influencing customer decisions, such as:
  - age
  - job type
  - balance
  - loan and housing status

> Note: Due to class imbalance, accuracy alone does not fully reflect performance on customers who said “yes”.

---

## 💡 Key Insights
- Not all customers should be contacted
- Certain customer groups are more likely to subscribe
- Data-driven targeting can reduce wasted calls and improve campaign efficiency

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
