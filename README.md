# Project Summary

## Synthetic Data Versions
Our project involves two versions of synthetic data for predicting **Risk Level** and **Loan Approval**.

### **Version 1: Large Feature Set**
- Contains **33 feature columns** plus **2 target columns** (Risk Level and Risk Score).
- Provides a detailed feature set but may be overly complex for real-world deployment.

### **Version 2: Reduced Feature Set**
- Contains **15 feature columns** plus **2 target columns** (Risk Level and Risk Score).
- Optimized for efficiency and reduced complexity while maintaining prediction performance.

---

## **Model Performance Comparison**

### **Version 1: Loan Approval Prediction**

#### Logistic Regression
- **Accuracy:** 91.45%
- **Precision, Recall, and F1-score:**
  - Approved (1): Precision **0.99**, Recall **0.78**, F1-score **0.87**
  - Rejected (0): Precision **0.88**, Recall **0.99**, F1-score **0.94**

#### Random Forest Classifier
- **Accuracy:** 91.00%
- Similar performance to Logistic Regression.

#### Gradient Boosting Regressor
- **Mean Squared Error (MSE):** 19.27
- **R² Score:** 0.76

---

### **Version 2: Risk & Loan Approval Prediction**

#### **Risk Level Prediction (Confusion Matrix & Report)**
- **Confusion Matrix:**
  - Low Risk: **86% Precision**, **76% Recall**, **81% F1-score**
  - Medium Risk: **92% Precision**, **93% Recall**, **93% F1-score**
  - High Risk: **85% Precision**, **85% Recall**, **85% F1-score**
- **Overall Accuracy:** 89%

#### **Loan Approval Prediction (Confusion Matrix & Report)**
- **Confusion Matrix:**
  - Approved: **76% Precision**, **77% Recall**, **76% F1-score**
  - Rejected: **76% Precision**, **75% Recall**, **75% F1-score**
- **Overall Accuracy:** 76%

---

## **Implementation in Django**
When implementing this model with Django, the focus will be on integrating the machine learning models into the fullstack. The setup process will not be emphasized, as the priority is on:
- Using **Django** for user inference easy for looking and input.
- User input the **data** in the form of the website the model is going to predict.
- **Serializing model predictions** into JSON responses.

---


## **Conclusion**
- **Version 1** provides high accuracy but requires more computational resources.
- **Version 2** simplifies the model while maintaining strong predictive power.
- **Django** Create the interface for user to input https://github.com/salarymakage/Loan-Advisor.git
