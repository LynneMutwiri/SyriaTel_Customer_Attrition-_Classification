# CUSTOMER CHURN CLASSIFICATION


![Graph](Img_One.png)


## Business Overview:
* Churn rate is the rate at which customers stop doing business with an entity. In telecommunications, it is expressed as the percentage of customers who discontinue their subscription in any given time period. A high churn rate means a service provider isn't able to retain customers; therefore, loyalty to their service is low.
* Churn could be as a result of poor customer experience or even a drop in the quality of services provided by the service provider. In this context, customer churn as also referred to as attrition rate or customer churn.

## Problem Statement
Build a classifier model that predicts the chances of customer churn and classifies a customer as either ```True```(soon to churn) or ```False```(not soon to churn).

## Business and Data Understanding 
* SyriaTel, a prominent telecommunications company operating in Syria, faces a common challenge in the industry: customer churn. After being in operation for over two decades, the smobile services provider faces a common risk of having both new and old customers discontinue their services and switch to competitors or opt for alternative solutions. In order to minimize churn and retain customers, SyriaTel recognizes the importance of identifying customers who are at high risk of churn, enabling them to take proactive measures to retain those customers.
* The most effective way to reduce the churn rate and consequently improve customer retention is making the most effective use of SyriaTel's internal data. The company has got very rich data which allows for better customer knowledge, to the point where they can collect them into precise and consistent segments and make conclusive analyses.
* Data used in this analysis is therefore from SyriaTel, since the stakeholder audience is SyriaTel stakeholders.

## Objectives:
* Identify most important features in the classification problem.
* Identify the best predictive model that classifies a customer as churn or not.
* Formulate recommendations to deal with customer churn.

## Modeling
For this project, machine learning was the most suitable form of data analysis. This is because this is a classification problem where the aim was to come up with a model that will make predictions on customer churn based on the history of customers. The model was trained on patterns, relationships, and statistical properties of input data and the corresponding output data, in this case churn. These past behaviours and characteristics were used to make predictions on the future of customer churn.
For the base model, ```Logistic Regression``` was used. Three other models were evaluated to compare their performances against the base model; ```decision trees```,``` random forests``` and ```XGBoost```.
The model that gave the best performance on both the train and test data was the ```Logistic Model```.

## Evaluation
* To evaluate the perfromance of the models, the best metric for this particular data was the ```Accuracy score```.
* A comparison to the ```AUC-ROC score``` was made to better understand the models' performances.
* Accuracy score is typically measured in the context of supervised machine learning tasks, specifically for classification problems. 
* It quantified the proportion of correct predictions(churn and not churn) made by the model out of the total number of predictions(false positives and false negatives).
* To enable the use of Accuracy score, the classes in the dataset had to be balanced since the data was imbalanced(non-churn outcomes were higher than churn outcomes).

## Conclusion
* The ```Logistic Regression``` model gave the highest and most consistent accuracy score on both the training and testing data.
* This means it will generalize well on new, unseen data compared to the other models such as random forest which seemed to overfit the data.
* In the futrure where more time is allowed for the project, ways to regularize and reduce overfitting will be applied to further evaluate the model(s).
