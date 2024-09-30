# Project Overview 


Fraud Detection Using Logistic Regression

This system detects if a financial transaction is fraudulent or not. I used a dataset containing transaction information and I applied various techniques to ensure the model's robustness. The main objective was to accurately classify transactions if they were fraudulent or non-fraudulent. The dataset contains the following features:

* Time: Time span between transactions.
* V1, V2, ..., V28: This are the Principal Component Analysis.
* Amount: The transaction amount.
* Class: This is the label which indicates whether a transaction is fraudulent or not.

Steps that were implemented 

1. Data cleaning.
2. Exploratory Data Analysis.  
3. Data Preprocessing: Due to the class imbalance between "fraudulent" and "non-fraudulent", I introduced the SMOTE (Synthetic Minority Over-sampling Technique) inorder to balance their values up. An imbalanced dataset can lead a model to be biased towards the majority Class. 
4. Model Selection: I chose Logistic Regression as the baseline model due to its ability to classify binary problems. 
5. Classification Report (Evaluation Metrics);
.   PRECISION: Precision measures the number of transactions the model flagged as fraudulent and are actually fraudulent. 
.   RECALL: Recall measures how well a model is able to identify true fraud. 
.  F1-Score: This is a balance between precision and recall. It gives a single metric that reflects both precision and recall. 
.  ROC-AUC Score: The Receiver Operating Characteristic curve and the Area Under the Curve helps to measure the model's measure ability to distinguish between fraudulent and non-fraudulent transactions.
. ACCURACY: Accuracy measures the performance of classification model. It is best used when the classes are balanced.


Shortcomings of Logistic Regression

Logistic Regression was unable to capture complex data present in fraudulent activities. It was yielding false positives (classifying a non-fraudulent transaction as fraudulent), leading to issues in real-world applications where accuracy is critical.
A more advanced algorithms like Random Forests, XGBoost, or Neural Networks could be used to help improve model performance.

Baseline Performance: The model provided a good starting point for fraud detection and can be improved by using more advanced techniques.
