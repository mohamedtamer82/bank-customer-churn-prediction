# bank-customer-churn-prediction
A supervised ML project focused on predicting churn based on bank customer data using Random-forest algorithm
# Bank Customer Churn Prediction 🚪📉

This project predicts which customers are likely to leave a bank (churn) using machine learning algorithms. It focuses on improving model performance, especially in identifying customers who are about to churn.

## 📌 Problem Statement

Customer churn is a major challenge for banks. Accurately predicting which customers are at risk of leaving helps the bank take proactive actions to retain them.

## 📁 Project Steps

1. **Data Preprocessing**
   - Loaded and explored the dataset.
   - Applied feature scaling.

2. **Handling Imbalanced Data**
   - Applied **SMOTE** (Synthetic Minority Oversampling Technique) to balance the classes.

3. **Model Training**
 - Random Forest Classifier

4. **Threshold Adjustment**
   - Used `predict_proba()` to change the decision threshold (from 0.5 to 0.3) to better identify churned customers.

5. **Model Evaluation**
   - Evaluated models using:
     - Accuracy
     - Precision
     - Recall
     - F1-Score
     - Confusion Matrix
     - ROC Curve

## 📊 Dataset

The dataset contains 10,000 customer records with features such as:
- Age
- Gender
- Geography
- Tenure
- Balance
- Estimated Salary
- Credit Score
- Churn label (Exited)

**Target Variable**: `Exited` (0 = stayed, 1 = churned)

## 🧠 What is SMOTE?

SMOTE stands for **Synthetic Minority Oversampling Technique**. It generates new synthetic examples of the minority class (churned customers) to balance the dataset and improve model performance.

## 📈 Final Model Performance

After using SMOTE, class weights, and threshold tuning:
- Accuracy: ~79%
- Recall for churn: significantly improved
- Balanced prediction between churned and non-churned customers

## 🛠️ Tools Used

- Python
- Pandas, NumPy
- scikit-learn
- imbalanced-learn
- Matplotlib, Seaborn
- Google Colab / Jupyter Notebook

## 🗂️ File Structure
## 📊 Results

After applying data balancing techniques (SMOTE + threshold tuning), the model achieved the following performance on the test set:

| Metric       | Class 0 (Not Churn) | Class 1 (Churn) |
|--------------|---------------------|-----------------|
| Precision    | 0.91                | 0.49            |
| Recall       | 0.82                | 0.70            |
| F1-Score     | 0.86                | 0.58            |
| Support      | 1593                | 407             |

**Overall Accuracy:** 79%  
**Macro Average F1-Score:** 0.72  
**Weighted Average F1-Score:** 0.80

- The model is better at identifying customers who will stay (`Class 0`).
- With SMOTE and threshold adjustment, recall for churners (`Class 1`) improved to **70%**, which is crucial in churn prediction use cases.

- 
## 📬 Contact

For questions or collaboration:

- **Mohamed Tamer**
- [LinkedIn](www.linkedin.com/in/mohamed-tamer-673ba82a9) 
- mohamedtamerr04@gmail.com



