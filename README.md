# Logistic regression credit risk classification

## **Overview**
 Logistic regression was used to develop a model based on loan risk, to identify the creditworthiness of borrowers, whether they are healthy or high risk.
 
Aspects to note:
 - X and y variables were created
 - Data was split into training and testing sets using the train_test split
 - Logistic Regression model created and fitted
 - Confusion matrix and classification report generated to evaluate the performance of the model
 
Two different logistic regression models were created:
 - The first using the original data set.
 - The second using resampled training data that over-sampled high risk loans (the minority group in this data set).

## **Outcome**
While both models accurately predict healthy loans, they differ in their ability to predict high risk loans.

In relation to high risk loans, though model 1 performed well, a key concern was the recall score (at 0.89), given the risk and potential cost to the business in misclassifying a high risk loan as healthy. However model 2 removed this concern, being able to accurately classify actual high risk loans as high risk (with a value of 1.00).

Both models score the same on precision in predicting high risk loans (at 0.87), meaning some healthy loans are being predicted as high risk. Which could potentially run the risk of losing business as a result.

Based on the analysis undertaken, model 2 (which used resampled training data) is the strongest performing model in predicting whether a loan is healthy or high risk. Given its performance I would recommend the company use model 2. But in recommending this I would ensure they were aware the model may incorrectly classify some healthy loans as high risk, so this could be an area they monitor. Future re-training of the model may also help to increase the precision in predicting high risk loans.<br/>
<br/>

---

### **Contact:**
Email: kymcoleman@gmail.com


---
<br/>

***Folder structure***


The folder 'Credit_Risk' contains:<br/>
 - '**credit_risk_classification.ipynb**' - contains two logistic regression models to identify the creditworthiness of borrowers.
 - '**report.md**' - comprehensive report on the analysis.