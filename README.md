# ADVANCED REGRESSION ASSIGNMENT

    # SUBMITTED BY DR RANJEET SINGH MAHLA

##DATE FEBRUARY 22, 2023

## MSC MACHINE LEARNING AND ARTIFICIAL INTELLIGENCE 


### KEY FILES
### Problem Statement1: jupyter notbook containing the assignment code (test train split and modelling with Lasso and Ridge): Part1_advanced_regression_assignment_RSM.ipynb
### data (train.csv file and data_description.txt) and data description file
### Problem Statement Part 2 (Questions Ashwers) pdf file: 

### 

## OVERVIEW
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file train.csv.

The company is looking at prospective properties to buy to enter the market. Objective is to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

## problem statement
The company wants to know:

    Which variables are significant in predicting the price of a house, and

    How well those variables describe the price of a house.

 
Also, the optimal value of lambda for ridge and lasso regression needs to be determined.

## Business Goal 
 
You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.


## Table of Contents
* [General Information](#general-information)
* [steps](#steps)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Acknoledgemenets](#acknoledgements)
* [contact](#contact)


<!-- You can include any other section that is pertinent to your problem -->

## General Information
- MULTIPLE LINEAR REGRESSION IS PERFORMED ON BIKE RENTAL DATA
- THIS PROJECT IS DONE TOWARDS AN ASSIGNMENT FOR MSC IN MACHINE LEARNING AND ARTIFICIAL INTELLIGENCE. 
- THIS PROJECT ESTIMATE THE KEY VARIABLES WHICH RELATE WITH BOOM BIKE RENTAL (some of the varaible represents to temperature, humidity, weather, holiday)
- IN THIS MODEL BOOM BIKE RENTAL DATA IS USED FOR BUILDING THE MODEL FOR BUSINESS RECOMMENDATIONS

### Steps 

    1) Reading, understanding and visualizing the data

    2) Preparing the data for model training (train-test split, rescaling)

    3) Training the model

    4) Prediction and evaluation of the test set with Ridge and Lasso regularization
    5) marking answers for assignment part 2



## Conclusions
- Data was refined for missing values and outliers (variables with more then 40% missing values were removed)
-null/missing/na values were replaced with median if there are outliers and mean when variable data was normally distributed
-EDA was perfomed on varaibles (continious and categorical) 
-highly skewd variables/column removed and least skwed column/variables adjusted by combining 
-data were splited to train and test model was created and best model was validated usinf Ridge and Lasso regularization to select final mdoel out of 5 fold validated models. 

For ridge regularization optimum value was 10 and for lasso optimum value was 0.00006

Top 5 predictors for Ridge
('GarageFinish_No Garage', 0.048),
 ('GarageFinish_RFn', 0.052),
 ('GarageFinish_Unf', 0.052),
 ('SaleCondition_Normal', 0.052),
 ('SaleCondition_Others', 0.057)


Ridge R2 values
- Train Score: 0.9048825126844456
- Test Score: 0.8762875068524612



Lasso regression: optimum alpha 0.00006
Top 5 predictors
('GarageFinish_No Garage', 0.051),
 ('GarageFinish_RFn', 0.066),
 ('GarageFinish_Unf', 0.072),
 ('SaleCondition_Normal', 0.074),
 ('SaleCondition_Others', 0.302)

Lasso R2 score 
- Train R2 Score: 0.9178195810624109
 - Test R2 Score: 0.883834546544181


## model is a robut model as R2(regression) value for train and test are very close and model is regularized with Ridge and Lasso, therefore it is a best robust and generalizable mdoel for unknown test data sets 

## Technologies Used
- matplotlib 3.7.0
- sci-kit learn 1.2.1
- numpy 1.24.2
- pandas 1.5.3
- seaborn 0.12.2
- jupyter notebook 5.2
- python 3.10
- matplotlib.pyplot 3.5.3


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## ACKNOLEDGEMENTS
The advanced regression project is creeated as part of MSC in AI and ML and as part of upgrad macine learning linear regression assignment. Thanks upgrad, iiitb and ljmu and the teachers 


## Contact
created by [@mahlaranjeet] feel free to contact me anytime at email given below
mahlaranjeet@gmail.com
