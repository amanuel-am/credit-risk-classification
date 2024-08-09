# credit-risk-classification
module 20 challenge

# overview
- use dataset of Historical lending activity from peer-to-peer lending services company and build a machine learning model to identify the creditworthiness of borrowers.
- data is split in 75% of the data going into the training set and 25% into the test set.
- Data trained with logistic regression model.
- Evaluation done with confusion matrix and model accuracy.

# result
- **Class 0 (Healthy Loan)**
  - **Precision: 1.00**
    - The model is perfect at predicting class 0. This means every loan predicted as healthy (0) is indeed healthy.
  - **Recall: 1.00**
    - The model correctly identifies all healthy loans. No healthy loans are missed.
  - **F1-Score: 1.00**
    - The F1-score, which is the harmonic mean of precision and recall, is perfect. This indicates a balance of precision and recall at their highest values.
  - **Support: 18,759**
    - The number of actual instances of healthy loans in the dataset is 18,759.

- **Class 1 (High-Risk Loan)**
  - **Precision: 0.87**
    - The model correctly identifies 87% of the predicted high-risk loans as actual high-risk.
  - **Recall: 0.89**
    - The model correctly identifies 89% of the actual high-risk loans. This means 11% of high-risk loans are missed.
  - **F1-Score: 0.88**
    - The F1-score indicates a good balance between precision and recall for high-risk loans.
  - **Support: 625**
    - The number of actual instances of high-risk loans in the dataset is 625.

- **Overall Metrics**
  - **Accuracy: 0.99**
    - The model has an overall accuracy of 99%, meaning 99% of the total predictions are correct.
  - **Macro Avg: 0.94 (Precision, Recall, F1-Score)**
    - The average metrics calculated without considering class imbalance are 0.94, indicating good performance for both classes when averaged.
  - **Weighted Avg: 0.99 (Precision, Recall, F1-Score)**
    - The average metrics considering class imbalance (more weight given to the healthy loans) are 0.99, indicating excellent overall performance.

# Summary
- **Interpretation**
  - The model performs excellently in predicting healthy loans (class 0), with perfect precision, recall, and F1-score.
  - For high-risk loans (class 1), the model performs well but not perfectly. It has a high precision of 0.87 and a high recall of 0.89, resulting in a strong F1-score of 0.88. This indicates that the model is quite good at identifying high-risk loans, although it does make some errors.
  - The overall accuracy of 99% suggests that the model is highly reliable, but it's important to note the class imbalance, as there are significantly more healthy loans than high-risk loans. Despite this imbalance, the model maintains strong performance across both classes.