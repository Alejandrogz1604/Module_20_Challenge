- This dataset consists of information on over 75 thousand loan applicants who have been classified as a poor or healthy loan risk. The dataset contains a series of features, such as "borrower income", "number of accounts", and a "debt to income" ratio. As a result of these features, the client has determined whether the borrower is a healthy loan risk, marked as "0" or negative, or a unhealthy loan risk "1" or positive with an increased chance of defaulting on their loan. Through machine learning, we have built a logistic regression model which will predict whether future applicants with similar characteristics as prior borrowers will have an increased probability of deffaulting on their lown.

- After splitting our dataset into training data for the model to learn on, and testing data to compare the accuracy of our predictions, we obtained the following results (as seen in our confusion matrix and classification report).
    - Healthy Loans:
        -Precision: 100%. Our logistic regression model has accurately predicted 100% of the true negative values (healthy loans) out of the true negative and false negative (positive) values. 
        - Recall 100%. We have correctly predicted 100% of the true negative values out of the true negative values and false positive (negative values).
     - Unhealthy Loans:
       -Precision: 87%. Our logistic regression model has accurately predicted 87% of the true positive values (unhealthy loans) out of the true positive and false positive (negative) values. 
        - Recall 89%. We have correctly predicted 89% of the true positive values out of the true positive values and false negative (positive values).
      - Accuracy Score: Overall, our logistic regression model has a 99.24% accuracy score, meaning that on average it is predicting values correctly 99.24% of the time.


- While our model has a significantly high accuracy score of 99.24%, I have a concern that I would want to discuss with my team prior to recommending this model to a client. While the model functions perfectly for predicting healthy loan risks, it´s precision and recall are significantly lower for predicting risky loan applicants.
- A recall of 89% when predicting unhealthy loan risks indicates that 11% of the loan applicants that were classified as unhealthy loan risks in our dataset, were predicted to be healthy loan applicants by our model. While 89% is a reletively good recall score, the 11% defficiency could lead to significant losses for the client in the long term.
  
