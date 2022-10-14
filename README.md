## Linear Regression Assignment on Bike Sharing

In this Bike Sharing assignment I am trying to build a multiple linear regression model for the prediction of demand for shared bikes. This assignment is to learn how to apply the Linear Regression concept of Machine Learning to find out relationship between variables.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- BACKGROUND : A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 
    
    In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


- PROBLEM STATEMENT : A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

    This assignment is to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 


- DATASET USED : The given dataset used "day.csv" for the assignment contains information about different factors that affect the demand of shared bikes i.e. the set of independent variables and dependent variable. 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- The independent variables 'atemp' and 'temp' are highly correlated  with the dependent variable 'cnt' and also highly correlated with each other which leads to multicolinearity hence, dropping 'atemp' and building the model with 'temp' and other independent variables.
- Most of the independent variables present in dataset are categorical and plays an important role in demand for bike sharing. Such independent variables are 'season',	'yr', 'holiday', 'weekday',	'workingday' and 'weathersit'. I have used MinmaxScaler technique of 'sklearn' Library for Normalizing this data.
- In this assignment I have used the approach where initially all the independent variables are passed to the model for prediction and then are dropped out based on the requirements of some of the model parameters pre-assumed values such as p-value, VIF.
- The model works fine in both training and testing phase. The  Residual Analysis check shows the Normal Distribution of the (y_train - y_train_pred) residuals. The model evaluation is done using calculating r2score of (y_test, y_test_pred) which is 0.7786089428454818.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python language is used for coding and Jupyter Notebook is used for that. Libraries used in python: pandas, numpy, matplotlib.pyplot, seaborn, sklearn, statsmodels.
- For collaboration, I have used Github platform.

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

- This assignment was done as part of the UpGrad course.
## Contact
Created by @DhanshreeVyas - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->