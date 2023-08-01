# Comprehensive-Bank-Customer-Analysis

This repository contains the code and analysis for comprehensive customer behavior analysis in a banking scenario. We perform three main tasks: customer segmentation, predicting whether a customer will subscribe to a term deposit, and predicting whether a customer will default on their loan.

## Dataset

The dataset used for this project is a bank marketing dataset. It includes customer demographic data (like job, marital status, education, age), as well as data related to loans (like whether they have a housing loan or personal loan), and data related to the last contact of the current campaign.

## Analysis and Results

### Customer Segmentation

We applied K-means clustering technique to perform customer segmentation. We grouped customers into clusters based on their age, job, marital status, education, default history, balance, housing loan, and personal loan. This segmentation helps in understanding the different customer groups and their behavior, allowing the bank to strategize their marketing and loan strategies accordingly.

### Term Deposit Subscription Prediction

We created several machine learning models to predict whether a customer would subscribe to a term deposit. Initially, we found that the dataset was imbalanced, which led us to use SMOTE (Synthetic Minority Over-sampling Technique) to balance it. 

After balancing the data and training the models, the XGB Classifier model performed best with an accuracy of 90%, precision of 59%, recall of 58%, F1 score of 59%, and ROC score of 76%.

### Loan Default Prediction

We also created several models to predict whether a customer would default on a loan. This dataset was also imbalanced, and despite applying SMOTE for balancing, the performance of the models was relatively low. 

The XGB Classifier model again performed the best, with an accuracy of 98%, precision of 20%, recall of 9%, F1 score of 12%, and ROC score of 54%. However, there is still room for improvement in these predictions, and more advanced techniques could be explored to enhance the performance.

## Implications

The results of these analyses can be valuable for banks in strategizing their marketing campaigns, risk assessments, and overall strategies for loan issuance and term deposit subscriptions.

## Future Work

Future work on this project could involve tuning the models for better performance, exploring different resampling techniques, and incorporating more features into the models to enhance their predictive power. It could also include more comprehensive customer segmentation using additional features.
