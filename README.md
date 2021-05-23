# ML-santander-customer-satisfaction


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
