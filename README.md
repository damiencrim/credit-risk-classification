# credit-risk-classification
Module 20 Challenge

For this Challenge, we used various techniques to train and evaluate a model based on loan risk. We imported a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

Utilizing the lending_data_csv which is comprised of several factors in determining a borrowers credit worthiness, ie: (loan size, interest rate, debt to income ratio as well as their total debt and derogaotry marks) which was then converted into a dataframe.

After splitting the data into Training and Testing functions we were then able to create a Logistic Regression Model to make predictions on the set. The initial set included a sampling of mostly Healthy Loans compared to High-Risk, 75,000 vs 2500, while the Oversampled set was more balanced at 56,271 counts for each category.

Results:

LRM_1-
 
 The Classification report for the testing data is :
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

 
 
 
 A balanced accuracy of 95% was achieved with the highlights falling in the Healthy Loan category scoring 100% in precision and F1 with a 99% Recall

 This model struggled in making predictions regarding High-Risk borrowers as it only achieved a Precision score of 85% with an F1 of 88%


 LRM_2

                precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384


A balanced accuracy score of 99% was achieved with the highlights again occurring in the Healthy Loan category returning 100% in Precision, 99% in Recall with an F1 of 99%

High-Risk scores saw a 1% drop in Precision yet the F1 improved by 3pts.



Summary: Overall, the model that utilized the Resampled Data outperformed it's counterpart in both Healthy and High-Risk loans. However, due to the importance of correctly predicting those that fall in the High-Risk category it is recommended that further trials be implemented in an effort to be more precise in those predictions.




