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
When implementing this model with Django, the focus will be on integrating the machine learning models into the backend API. The setup process will not be emphasized, as the priority is on:
- Creating **API endpoints** for model inference.
- Handling **data preprocessing** before feeding inputs to the model.
- **Serializing model predictions** into JSON responses.
- Implementing **asynchronous requests** for efficiency in model execution.
- Ensuring **security** in handling user data and predictions.

Django REST Framework (DRF) will be used for building the API, and joblib will be utilized to load pre-trained models efficiently.

---

## **User Interface & Application Flow**
Below are some screenshots showcasing the user interface for the loan application and loan details:

### **Loan Application Form**
![Loan Application Form](image/Screenshot%202025-02-07%20101508.png)

### **Loan Approval Details**
![Loan Approval Details](image/Screenshot%202025-02-07%20101615.png)

### **Loan Summary View**
![Loan Summary View](image/Screenshot%202025-02-07%20101615.png)

---

## **Conclusion**
- **Version 1** provides high accuracy but requires more computational resources.
- **Version 2** simplifies the model while maintaining strong predictive power.
- **Django** Create the interface for user to input. m 
