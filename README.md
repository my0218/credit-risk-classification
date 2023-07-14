# credit-risk-Analysis-Report
Overview:
The purpose of this analysis is to make prediction on loan status (healthy or high-risk) based on various features of the loan. The analysis is ultilizing logistic regression model by training it to use the data and making predictions. To test the module performance, we also resampled the data by via RandomOverSampler and made comparison.


Results:
1. Logistic Regression Model with Original Data:
   --Accuracy Score: The accuracy score of the model on the testing data is 0.99 on f1-score.
   --Precision Score: The precision score for the healthy loan (label 0) is 1.00, indicating that all predicted healthy loans are correct. For high-risk loans (label 1), the precision score is 0.87, suggesting that 87% of predicted high-risk loans are correct.
    --Recall Score: The recall score for both healthy loan (label 0) is 1.00 while the one for high-riak loan (label 1) is 0.89 indicating that the model correctly identifies all instances of healthy loan but lower instances of high-risk loan.

2. Logistic Regression Model with Resampled Training Data:
   --Accuracy Score: The accuracy score of the model on the testing data is 1.0 on f1-score.
   --Precision Score: The precision score for the healthy loan (label 0) is 1.00, indicating perfect precision. For high-risk loans (label 1), the precision score is 0.87, suggesting that 87% of predicted high-risk loans are correct.
  --Recall Score: The recall score for both healthy loan (label 0) and high-risk loan (label 1) is 1.00, indicating that the model correctly identifies all instances of both classes.


Summary:
The logistic regression model performs well in predicting both healthy loans and high-risk loans, whether with the original data or the resampled data. The model achieves perfect precision, recall, and high accuracy for healthy loans (label 0) in both cases. For high-risk loans (label 1), the model shows slightly lower precision (87%) but maintains perfect recall. This indicates that the model can accurately identify high-risk loans, but there may be some false positives.

Based on the performance metrics and results obtained from both models, it is recommended to use the logistic regression model with resampled training data. This model addresses the class imbalance issue through random oversampling, resulting in improved performance on high-risk loans. The model's high precision and recall scores for both classes demonstrate its effectiveness in predicting loan status. However, it is important to note that the recommendation is based solely on the performance of the logistic regression model, and other factors specific to the business context should be considered before finalizing the model for deployment.

