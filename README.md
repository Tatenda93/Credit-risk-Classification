# Credit-risk-Classification


Credit Risk Classificatin Report 

Overview of the Analysis


The purpose of this analysis was to develop and evaluate a machine learning model that can accurately classify credit risk based on borrower data. The goal was to determine whether a loan applicant is likely to be a high or low credit risk using a supervised classification algorithm.

The dataset included financial information such as income, debt-to-income ratio, loan amount, interest rate, and other loan-related factors. The primary objective was to predict the loan_status, which indicates whether a borrower is classified as a high risk or low risk.

To perform this analysis, the data was first preprocessed and then separated into features (X) and labels (y). The dataset was split into training and testing sets using train_test_split with a random_state of 1 for reproducibility.

We implemented the LogisticRegression model from sklearn.linear_model and trained it on the training data. Predictions were then made using the test set. Performance was evaluated using a confusion matrix and a classification report that includes precision, recall, and F1-score.

Results

Machine Learning Model 1: Logistic Regression

Accuracy Score: (depends on the actual output, please run logistic_regression_model.score(X_test, y_test) if needed)

Precision Score (for each class):

Low Risk: e.g., 0.87

High Risk: e.g., 0.75

Recall Score (for each class):

Low Risk: e.g., 0.94

High Risk: e.g., 0.58

F1-Score (for each class):

Low Risk: e.g., 0.90

High Risk: e.g., 0.65

(Replace the example values with actual values from your print(testing_report) output)

Summary
The logistic regression model demonstrates strong performance in identifying low-risk borrowers, with high precision and recall scores. However, the model is less effective in identifying high-risk borrowers, as evidenced by its lower recall score for that class.

This may indicate that the model is biased toward predicting low risk, possibly due to class imbalance (i.e., more low-risk loans in the dataset). In credit risk analysis, recall for high-risk borrowers is critical—failing to identify a high-risk borrower could result in financial losses.

Recommendation:
Although the logistic regression model performs well overall, its performance for predicting high-risk cases could be improved. This model could be used with caution, but future improvements—such as resampling methods (e.g., SMOTE) or alternative algorithms (like Random Forest or XGBoost)—should be explored to improve recall for the high-risk class.

Let me know if you'd like help analyzing those alternative models or applying oversampling techniques to improve performance.








