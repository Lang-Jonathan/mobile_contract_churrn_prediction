# Mobile Contract Churn Prediction
## Project description
The fictive telecom operator *Interconnect* would like to be able to forecast their churn of clients. If it's discovered that a user is planning to leave, they will be offered promotional codes and special plan options.  
Therefore, Interconnect's marketing team has collected some of their clientele's personal data, including information about their plans and contracts.  
Based on this data a machine learning algorithm with a minimal AUC-ROC score of 0.79 should be developed.

## Content
In this project the following steps have been carried out:

- Developing an project plan
- Data loading, merging and inspecting
- Extensive data preprocessing
- In-depth Exploratory Data Analysis
- Feature engineering
- Multiple approaches on dealing with class imbalance
- Model evaluation with crossvalidation
- Model building, training and evaluation of multiple algorithms via pipeline
- Multi-iteration hyperparameter tuning

## Outcome
Performance of the Algorithms:  

- LightGBM turned out to be the best (of the considered algorithms) fitting classifier for this problem
- The final model has an AUC-ROC score of round about 95% and is  sufficient to predict the customers, who are going to churn. This gives telecom the chance to offer those clients special deals which might change their minds to stay 
- For the tree based models standard scaling could have been skipped. Same applies for the categorical frequency encoding for regressors like LGB and XGB

For binding the customers to the company the following measures are proposed:

- checking why the Churns started in Oktober 2019 and take measures against the cause
- Trying to bind new clients more to the company cause once they stay for a longer time they are more likely to stay
- Try to up-sell their additional services especially streaming cause it makes churns unlikely
- Try to sell more cheep contracts cause those customers are more unlikely to churn
- Use the developed model to check who is going to churn and make those clients offers in advance