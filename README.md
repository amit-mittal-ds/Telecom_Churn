# Telecom_Churn

## Problem Statement
A telecom company wants to know whether a particular customer will switch to different service provider or not (Churn or not). They have some some previous data of customer who churns and did not churned like monthly recharges, online services they are availing, customer demographics etc.
Company also needs to know the factors which influences the customer to churn and how much is the impact of those factors. Through this company will focus to improve in those area to retain their customers. They needs a descent model that can predict good percentage of Churn and Non-Churn customer correctly.

## Approach Used
Since this is a binary classification problem, I preffered to use logistic regression model because it works good for binary classification problems and is easy to interpret which is import in this case as the company wants to know the impact for factors influencing churn.

1. We got 21 variables explaining the customer relation with the company.
2. First, I did some preprocessing steps to make the data ready for the model and got 23 variables.
3. Then, I used Recursive Feature Elimination (RFE) to choose top 15 features for initial model.
4. We used Back-propogation technique to eliminate features based on p-value and Variable Inflation Factors (VIF).
5. Finally came up with the final model with 12 variables.
6. Evaluated model performance on the training set and choose best cut-off value.
7. Tested the model performance on testing set for validation.
8. Interpreted the variable coefficients

## Conclusion
The model gave good accuracy score of 77% on the Training dataset and 74% on the Testing dataset along with other metrics (sensitivity and specificity) i.e. a descent model that can predict good percentage of Churn and Non-Churn customer correctly, as per client's requirement. We got to know that,
- A customer with long term contracts like One year and Two Year are less likely to churn than the customer having Monthly contract
- A customer who is associated with the company from longer time is less likely to churn than a customer who is associated from few months. Reason can be the customer is happy with the services and wishes to continue with them
- Customer using Internet Services, Fiber Optics, Streaming TV and Movies servies are more likely to churn than customer who are not using these services. Reason can be company not providing good Internet services and need to work on that.
- Customer who have opted for Payment Method through Credit Card or Mailed check are less likely to churn then other customers.

#### Overall, company need to provide better internet services and other services associated with internet to retain their customers.
