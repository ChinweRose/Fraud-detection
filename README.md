#Project Overview

## Fraud-detection

This project focuses on building a predictive model to detect fraudulent financial transactions. We used a dataset containing transaction information and applied various data preprocessing techniques to ensure the model's robustness. The main objective was to accurately classify transactions as either fraudulent or non-fraudulent.

###Dataset
The dataset contains the following features:
Time: Time elapsed between this transaction and the first transaction.
V1, V2, ..., V28: The principal components obtained through PCA.
Amount: The transaction amount.
Class: The label indicating whether the transaction is fraudulent (1) or not (0).

##Procedures
. Data Preprocessing
Handled class imbalance using SMOTE (Synthetic Minority Over-sampling Technique) to balance the number of fraudulent and non-fraudulent transactions.
Split the dataset into training and testing sets using an 80-20 split.
2. Model Selection
We chose Logistic Regression as the baseline model due to its simplicity and interpretability.
Logistic regression was used to predict the probability of a transaction being fraudulent or not.
3. Evaluation Metrics
Precision: Precision measures the proportion of true fraud predictions among all transactions predicted as fraud.
Recall: Recall measures the proportion of actual fraudulent transactions that were correctly predicted.
F1-Score: A balance between precision and recall, useful for assessing the model’s performance when the dataset is imbalanced.
ROC-AUC Score: The Receiver Operating Characteristic curve and the Area Under the Curve helped us measure the model’s ability to distinguish between fraudulent and non-fraudulent transactions.
Classification Report: Provided a detailed breakdown of precision, recall, F1-score, and support for both classes (fraud and non-fraud).
4. Shortcomings of Logistic Regression
Logistic regression assumes linearity between the features and the log-odds of the outcome, which may not always hold for complex fraud patterns.
It may struggle to capture the subtle, non-linear relationships present in fraudulent activities.
The model may yield false positives (classifying a non-fraudulent transaction as fraudulent), leading to issues in real-world applications where accuracy is critical.
5. ROC Curve
The ROC curve provided a visual representation of the trade-off between True Positive Rate (Recall) and False Positive Rate.
The ROC-AUC score was a key indicator of the model's performance. A score closer to 1 indicated good model performance.
6. Model Strengths
Interpretability: Logistic regression provides clear insights into how different features contribute to the probability of a transaction being fraudulent.
Speed: It’s computationally efficient and quick to train.
Baseline Performance: The model provides a good starting point for fraud detection and can be improved by using more advanced techniques.
7. Limitations
While logistic regression gave decent performance, it failed to capture non-linear patterns, which are often present in complex fraudulent transactions.
In the future, using more advanced algorithms like Random Forests, XGBoost, or Neural Networks could help improve model performance.
Conclusion
This project demonstrates how logistic regression can be applied to a fraud detection problem. Although the model performed reasonably well, more advanced models or feature engineering may be required to further improve fraud detection accuracy.


