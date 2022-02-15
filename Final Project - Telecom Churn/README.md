# Telecom Churn Project

## Task Statement
The telecom operator Interconnect would like to be able to forecast their churn of clients.
If it's discovered that a user is planning to leave, they will be offered promotional codes and special plan options.
Interconnect's marketing team has collected some of their clientele's data, including information about their plans and contracts.



## Description of the data

### `contract` table:
- `customerID` - The ID of the customer.
- `BeginDate` - Beginning date of the contract.
- `EndDate` - End date of the contract.
- `Type` - Type of contract (monthly, yearly, bi-yearly)
- `PaperlessBilling` - Billing through e-mail.
- `PaymentMethod` - The method of payment.
- `MonthlyCharges` - Monthly charges.
- `TotalCharges` - Total charges.

### `personal` table:
- `customerID` - The ID of the customer.
- `gender` - Gender of the customer.
- `SeniorCitizen` - Is the customer a senior citizen?
- `Partner` - Does the customer have a partner?
- `Dependents` - Does the customer have children?
				
### `internet` table:
- `customerID` - The ID of the customer.
- `InternetService` - Does the customer use internet service?
- `OnlineSecurity` - Does the customer use an online security service?
- `OnlineBackup` - Does the customer use an online backup service?
- `DeviceProtection` - Does the customer use a device protection service?
- `TechSupport` - Does the customer use tech support service?
- `StreamingTV` - Does the customer use a streaming TV service?
- `StreamingMovies` - Does the customer use streaming movies service?
	
### `phone` table:
- `customerID` - The ID of the customer.
- `MultipleLines` - Does the customer use multiple lines of a phone?
<br>


## Summary
In this project, we studied data provided by a telecom company to train a model that would predict the churn of clients.
The company would like to know in advance which customer is more likely to churn so they could offer benefits to encourage the customer to stay active, a binary classification problem.

### Challenges
There were quite a few challenges in this project regarding data preparation and pre-processing.
- Not all of the provided data sets were of the same length, as a result, the merge of these tables produced NaN values in various services in over 20% of the data. That is significant, moreover that it is not a large data set.
- The data represented a class imbalance between customers that already left (the minority) to data on clients that are still active (the majority)
- Training and optimizing different models to reach the required threshold, building a pipeline, using GridSearchCV to identify the best hyperparameters combination and an evaluation function for each model.
