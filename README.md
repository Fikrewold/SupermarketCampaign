Supermarket marketing campaign Case Study.¶
Session Agenda
•	Understand the basic concepts of Hyperparameter tuning and pipelines
•	Learn how to use RandomisedCV for model tuning, to reduce the time-complexity involved in Grid Search CV
•	Learn feature importance using a new package called “SHAP” to make the model more interpretable.
•	Understand how pipeline with column transformer can help standardize the model building process
•	Learn about industrial applications of these techniques

Context
'All You Need' Supermarket is planning for the year-end sale. They want to launch a new offer - gold membership for only $499 which is \$999 on normal days(that gives a 20% discount on all purchases).
It will be valid only for existing customers, they are planning to start a campaign through phone calls.
The best way to reduce the cost of the campaign is to make a predictive model which will classify customers who might purchase the offer, using the data they gathered during last year’s campaign.
We will build a model for classifying whether customers will reply with a positive response or not.
So far we have used various machine learning algorithms to make predictive models. In this session, we would go a little deeper and understand how we can improve the model performance by tuning certain hyperparameters. After building an Ml model, we will identify the contribution of each factor in making predictions. And finally, we will learn how to standardize the ml models using a pipeline. Let's list out a few objectives for the case study.

Objective
•	Identify different factors that impacts the response of the customers.
•	Improve the model performance using hyperparameter tuning.
•	Build pipeline to standardize the training process.

Data Description
•	Response (target) - 1 if customer accepted the offer in the last campaign, 0 otherwise
•	ID - Unique ID of each customer
•	Year_Birth - Age of the customer
•	Complain - 1 if the customer complained in the last 2 years
•	Dt_Customer - date of customer's enrollment with the company
•	Education - customer's level of education
•	Marital - customer's marital status
•	Kidhome - number of small children in customer's household
•	Teenhome - number of teenagers in customer's household
•	Income - customer's yearly household income
•	MntFishProducts - the amount spent on fish products in the last 2 years
•	MntMeatProducts - the amount spent on meat products in the last 2 years
•	MntFruits - the amount spent on fruits products in the last 2 years
•	MntSweetProducts - amount spent on sweet products in the last 2 years
•	MntWines - the amount spent on wine products in the last 2 years
•	MntGoldProds - the amount spent on gold products in the last 2 years
•	NumDealsPurchases - number of purchases made with discount
•	NumCatalogPurchases - number of purchases made using catalog (buying goods to be shipped through the mail)
•	NumStorePurchases - number of purchases made directly in stores
•	NumWebPurchases - number of purchases made through the company's website
•	NumWebVisitsMonth - number of visits to company's website in the last month
•	Recency - number of days since the last purchase
Sklearn provides various libraries to build models and assess the performance. Let's import the packages

