# Auto-Insurance-Crash-and-Cost-Prediction
Predicted the likelihood of auto insurance customers getting into a car accident using logistic regression in R and estimated the costs of these crashes using linear regression.


# Predicting the Likelihood of Car Crashes and the Cost of those Crashes for Auto Insurance Customers

## Author
Teddy Kelly

## Overview

This project uses an auto insurance dataset to predict the likelihood that a customer gets
into an accident and if so, estimates how much that crash costs given provided information 
about each customer's age, income, gender, number of traffic violations, etc.).
Additionally, the project identifies which variables are most determinant of signaling
if a customer is at risk for getting into an accident.

## Other Files
Auto_Insurance_Crash_Prediction.qmd
- R quarto file that contains all of the code used for the project.
  
Auto_Insurance_Crash_Prediction.pdf
- Paper containing exploratory data analysis, data visualizations, data cleaning,
methodology, regressions, results, and interpretations.


## Data
- Training Data: insurance-training-data2-2.csv
- Testing Data: insurance-testing-data2-2.csv
- In total, the training and testing data contain approximately 8,000 records with each one
representing a customer at a car insurance company.
- 1st Dependent Variable: `crash flag` - Binary variable where a 0 represents that a
customer was not in an accident and a 1 means they were in an accident.
- 2nd Dependent Variable: `log crash cost` - A log transformation of how much each accident
cost since the crash cost data were heavily skewed to the right.
- 23 predictor variables with the main ones being `age`, `car age`, `car type`, `income`,
`number of kids driving`, license revoked`, etc`

## Methods
- Logistic regression to predict the likelihood of a crash occurring
- Multivariate linear regression to predict the cost of each crash
- Confusion matrices to evaluate model prediction accuracy of logistic regression
- Diagnostic testing and residual analysis to confirm model validity of multivariate regressions.

## Tools
- R Studio(tidyverse, ggplot2, glm, stargazer)

## Results
- The 2nd logistic regression was the model for prediction with an accuracy rate of about 79%
- People working in urban areas, single parents, unmarried people, sports car owners, teen drivers,
and people with more traffic violations were among the most notable groups of customers to have
higher crash likelihoods.
- The 2nd linear model was the best for making predictions on crash payout values.
- Unmarried customers, customers with lots of traffic violations, and customers with expensive
cars were among the most notable variables to be positively associated with higher crash costs.
- The 2nd linear regression with the log transformation of crash costs had a mean and median
crash cost prediction of about $3,939 and $3,952 respectively, indicating a very symmetric
distribution. 



