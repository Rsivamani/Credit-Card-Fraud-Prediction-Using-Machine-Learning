

# **Credit Card Fraud Prediction Using Machine Learning**

## **Summary**

This project solves the problem of accurately detecting rare fraudulent credit card transactions from highly imbalanced data while minimizing false positives and financial loss

## **Project Overview**

Credit card fraud poses a significant financial risk to both businesses and consumers. This project focuses on building a machine learning–based classification system to identify fraudulent credit card transactions using historical transaction data.

The dataset used is publicly available on **Kaggle**, consisting of **284,807 transactions**, of which only **492 are fraudulent**. Due to this extreme class imbalance, specialized preprocessing and evaluation techniques were required to ensure reliable model performance.

---

## **Problem Statement**

To develop a robust machine learning model capable of accurately predicting fraudulent credit card transactions while minimizing false positives, despite severe class imbalance in the dataset.

---

## **Methodology**

The project followed a structured data science workflow:

1. Data understanding and exploration
2. Data cleaning and validation
3. Exploratory Data Analysis (EDA)
4. Feature preparation and transformation
5. Train–test split
6. Model training and hyperparameter tuning
7. Model evaluation and comparison

---

## **Data Preprocessing**

Key preprocessing steps included:

* **Missing Values**:
  The dataset contained no missing values.

* **Outlier Treatment**:
  No explicit outliers were detected that required removal or transformation, as most features were already PCA-transformed.

* **Class Imbalance Handling**:
  Fraudulent transactions accounted for only **0.172%** of the data. To address this imbalance, **SMOTE (Synthetic Minority Oversampling Technique)** was applied to the training data to improve the model’s ability to learn minority class patterns.

---

## **Model Development**

The following machine learning algorithms were trained and evaluated:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

Hyperparameter tuning was performed to optimize model performance.

---

## **Evaluation Metrics**

Given the imbalanced nature of the dataset, multiple metrics were used:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC–AUC

This ensured balanced assessment of both fraud detection capability and false positive control.

---

## **Model Performance**

| Model               | Accuracy | Precision | Recall | F1 Score | ROC AUC |
| ------------------- | -------- | --------- | ------ | -------- | ------- |
| Logistic Regression | 99.83%   | 99.82%    | 99.41% | 99.61%   | 99.95%  |
| XGBoost             | 99.84%   | 99.82%    | 99.52% | 99.67%   | 99.96%  |
| Decision Tree       | 99.82%   | 99.81%    | 99.38% | 99.59%   | 99.94%  |
| Random Forest       | 99.83%   | 99.82%    | 99.43% | 99.62%   | 99.95%  |

---

## **Results and Insights**

All models demonstrated strong performance across evaluation metrics. However, **XGBoost consistently outperformed the other models**, achieving the highest accuracy, recall, F1 score, and ROC–AUC.

This indicates that XGBoost is particularly effective at capturing complex patterns in highly imbalanced fraud detection data.

---

## **Conclusion**

The **XGBoost model** emerged as the most effective solution for credit card fraud detection in this project. Its high recall and precision demonstrate a strong ability to identify fraudulent transactions while maintaining a low false positive rate.

---

## **Cost–Benefit Analysis**

* **Implementation Cost**: Low
  XGBoost is open-source and computationally efficient.

* **Business Benefit**: High
  Early detection of fraudulent transactions reduces financial losses, operational risk, and customer dissatisfaction.

---


