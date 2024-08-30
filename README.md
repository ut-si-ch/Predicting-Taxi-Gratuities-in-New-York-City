# Predicting-Taxi-Gratuities-in-New-York-City
Used multiple linear regression to predict taxi fares, data that would be used as a part of a suite of models to optimize revenue for the New York City Taxi and Limousine Commission and its drivers.

# Overview
The goal of this project was to create a multiple linear regression and random forest model to predict high rider gratituity or not. This project utilized yellow taxi trips taken in New York City during 2017. The final random forest model performed with 86% accuracy and 72% precision determining what features were most important in separating low tippers from high tippers. Based on the model, the duration, distance and cost of the trip were most influential in determining a generous tipper(>20%) vs a non-generous one(<20%).  

# Business Understanding
According to salary.com the average salary for a New York Taxi Driver is around $45000. This salary is significantly low compared to a median rent value of $6500 per month. It is important to understand what factors encourage riders to leave tips in order to help drivers obtain a livable wage.

# Data Understanding
The NYC Taxi and Limousine Commission data come from NYC.gov. The data consisted of approximately 408k unique tips and 18 features.The features included information on trip duration and destination, vendor used, toll information, and payment type.The bar chart below shows the breakdown of how many generous tippers(>20%) versus non-generous tippers(<20%) that exist in the data set.
![image](https://github.com/ut-si-ch/Predicting-Taxi-Gratuities-in-New-York-City/assets/83574378/a0ada1e4-469d-434b-9a9d-e0ca455cc59c)


In connection to this, a feature was engineered to represent if a ride was taken during rush hour or not. Multiple redundant columns were dropped and were formatted into the proper data type.


# Modelling and Evaluation
A random forest model comprising 100 decision trees were used to determine feature importance in who would tip generously or not. The below plot shows that trip duration, distance, and the cost of a fare were the TOP 3 most important factors in determining a generous tipper from a non-generous one. The overall model performed with 64.5% accuracy and 36.5% precision.
![image](https://github.com/ut-si-ch/Predicting-Taxi-Gratuities-in-New-York-City/assets/83574378/2159a8b4-daab-4e73-ba36-922ed62ad1a9)
This is not a great model, but depending on how it's used it could still be useful. If the objective is only to help give taxi drivers a better idea of whether someone will leave a good tip, then it could be useful. It may be worthwhile to test it with a select group of taxi drivers to get feedback.


# Conclusion
This model can benefit Taxi drivers in knowing if they will be tipped generously or not; however, running a parametric model to determine how much each variable will influence the actual price of the tip. In the future, adding more information on a rider's past tipping behaviour in helping the stakeholder address their business problem.
