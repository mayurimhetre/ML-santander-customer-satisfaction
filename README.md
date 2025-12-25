# Santander Customer Satisfaction Dataset

## Overview
The **Santander Customer Satisfaction** dataset comes from a Kaggle machine learning competition. The goal is to predict whether a customer is **satisfied or dissatisfied** with Santander Bank services based on anonymized customer features.

## Objective
Build a classification model to identify **unhappy customers** early, allowing the bank to take proactive actions to improve customer retention.

---

## Dataset Description
- Each row represents a **customer**
- Features are **anonymized numerical variables**
- The target variable is **`TARGET`**:
  - `0` → Satisfied customer
  - `1` → Dissatisfied customer

---

## Key Characteristics
- High-dimensional dataset (hundreds of features)
- Strong **class imbalance** (more satisfied than dissatisfied customers)
- No missing values, but many **constant and redundant features**

## Common Challenges
- Handling imbalanced classes
- Removing low-variance features
- Preventing overfitting due to high feature count

## Implementation

PCA (Principal Component Analysis) is a dimensionality reduction technique that transforms correlated features into a smaller set of uncorrelated components while preserving most of the data variance.
In this dataset, PCA helps reduce noise and redundancy, improving model efficiency and reducing overfitting.

---

## Results 
**1. PCA - 2 components:**

**Random Forest Classifier Used:**

![image](https://user-images.githubusercontent.com/68188457/119265515-af304780-bc04-11eb-84df-1f771b0283e7.png)

NOTE:
Records - 375 -- detected as 1 that means customers are unsatisfied.


Given in problem set :
You are provided with an anonymized dataset containing a large number of numeric variables. The "TARGET" column is the variable to predict. It equals one for unsatisfied customers and 0 for satisfied customers.
1: unsatisfied customers
0 : satisfied customers
    
The task is to predict the probability that each customer in the test set is an unsatisfied customer.
in sample_submission op: 0 for 75818 records.

**ACCURACY : 99.50 % is achieved**.



**2. PCA - 2 components:**

Random forest used after hyperparameter tuning:

criterion='entropy', max_depth=10, max_features='log2',min_samples_split=3, n_estimators=6

![image](https://user-images.githubusercontent.com/68188457/119265956-742f1380-bc06-11eb-98f3-2bf75852f9e3.png)


Records - 0    -- detected as "1"
Records - 75818 - detected as "0"

**Accuracy: 100 % achieved.**
