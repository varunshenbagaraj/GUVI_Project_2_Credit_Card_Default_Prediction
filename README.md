## GUVI_Project_2_Credit_Card_Default_Prediction

### Problem Statement
Financial threats are displaying a trend about the credit risk of commercial banks as the incredible improvement in the financial industry has arisen. In this way, one of the biggest threats faced by commercial banks is the risk prediction of credit clients. The goal is to predict the probability of credit default based on credit card owner's characteristics and payment history.

### Tools Used
* Programming Language – Python
* Data Analysis – Pandas
* Data Visualization – Matplotlib, Seaborn
* ML Algorithms – Logistic Regression, Decision Tree Classifier, Random Forest Classifier, Support Vector Classifier, KNN Classifier
* Performance Evaluation – AUROC, Accuracy Score

### Approach
* Since the problem statement is a Binary classification type, Logistic Regression, Support Vector Classification, KNN Classification, Decision Tree and Random Forest Classification were used.
* All the features were renamed for better readability.
* The independent variables were scaled using StandardScaler irrespective of the algorithm.
* The results of prediction was evaluated using Accuracy score and AUROC.
* Since AUROC is the best metric for classification problems, the best model was selected based on AUROC score.
Important  features(i.e. strongest predictors) were chosen from the coefficients(weights) and attributes available within the model. Feature importance was computed for every algorithm to double check.
* Evaluation metrics and Feature importance have been tabulated.

### EDA Insights
* Most people have a credit limit of 50000 New Taiwan Dollars
* People aged in the late 20’s use credit cards the most
* The defaulters are very less compared to non-defaulters. This indicates that the dataset is imbalanced. However, this aspect is not covered in this project.
Females have defaulted more than males
* The number is defaulters who are married is only slightly higher than those who are single.
* People who went to university have defaulted the highest
* The status of payment from April to September 2005 (As_on_April_05…As_on_Sep_05) are the only set of variables that have a positive effect on the target variable (Next_Month_Default)

### Best Model - Decision Tree
Decision Tree Classifier and Random Forest Classifier have given nearly same training and testing accuracy scores.
The best model was selected based on AUROC score i.e. Decision Tree
> * Decision Tree = 0.661
> * Random Forest  = 0.652

### Evaluation Metrics of the best model - Decision Tree Classifier
> * Training Score = 0.828
> * Testing Score= 0.818
> * AUROC = 0.661
