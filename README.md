# House_price_predictive_analysis
Regression analysis to predict the price of house using independent variables


## Introduction
This analysis is meant to understand the influence of significant variables on the price of a house and how well these variables can be used to predict the price of the house


## Aims and objectives
1. This analysis is aimed at identifying diffderent variables that contribute to the price of the house
2. Understanding how much variance in the  dependent variable that can be attributed to the independent variable
3. Developing a model that could accurately predict the price of the house in this dataset


## Understanding the data structure
This dataset is gotten from Kaggle. This dataset contains the price of the house as well as other significant variables. Other significant variables can be seen below:

1. Square feet

2. Bedroom

3. Bathroom

4. Neighbourhood

5. Year Built

6. Price

By understanding the data structure, correlation analysis was done to determine the relationship between these variables and the price of the house. This analysis will provide insights into the factors that may influence the prices of the house as well as the dynamics of the house market.

## Tools
The tools used for this analysis was Microsoft Excel together with the add-in in Excel

## Data Cleaning and Preparation
•	The dataset was imported as a csv format and converted to an excel format using text to columns 

•	The Price column value was converted from 2 decimal places to whole numbers

## Correlation and multiple linear regression analysis

**Numerical Variables**

The dataset contains 5 numerical variables and correlation analysis was performed on them to determine the relationship between these variables and the dependent variable(Price) and how strong the relationships are. The dependent variable was purposely ommitted to focus on the relationships between the other variables and the dependent variable.


Square feet	| 0.7507| 	Strong positive correlation

Bedroom	| 0.0726| 	Weak positive correlation

Bathroom	| 0.0284| 	Weak positive correlation

Year Built	| -0.0023| 	Weak negative correlation

**Significant numerical variable after correlation analysis**

• Square feet

**Categorical Variables**

The dataset conatains 1 categorical variable and it was converted to dummy variable and regression analysis was performed on it.


## Final regression analysis result
The multiple-R value of **0.75** shows that there exist a strong relationship between the variable and the house price. The *R square* value shows that **57%** of variance in the house price is influenced by the independent variable which is squarefeet. The *p-value* strongly agree with this with a p-value of 0. 

However, 43% of variance in the dependent variable can be attributed to other variables not in the dataset.

**Linear Regression Model Equation**

Dependent variable(House price) = Coefficient of Intercept + (99.322 * Squarefeet) 

**Testing the model using prediction**
• Squarefeet: 2126

**Using the regression model equation**
Dependent variable(House price) = Coefficient of Intercept + (99.322*Squarefeet) 

H = 25549.96 + (99.322 * 2126) 

H = 25549.96 + 211,158.57

H = 236,708.53

H = 236,709

**Predicted price** : 236,709

**Actual price** : 215,355

The predicted price is 21,354 higher than the actual price


## Actual Price vs Predicted Price

![Screenshot 2024-07-10 175920](https://github.com/NStanley0524/House_price_prediction_analysis_Excel/assets/169830658/221abb04-301c-406e-b70d-9312c6328d5d)



## Conclusion
The analysis above shows that Square feet has significant impact on the price of a house. The variable also showed positive relationship of 0.75 on the corellation analysis to the price of a house which means that the bigger the squarefeet, the higher the price of the house. Other numerical variables like Bedroom,Bathroom and Year built were not included in the final regression analysis because they lack statistical significance.

The analysis also shows that the cathegorical variable, neighbourhood does not have any influece on the price of a house. Their analysis showed weak relationship to the price of the house and their contribution to the variance of the dependent variable was negligible.

Futhermore, 47% of the remaining variance on the dependent variable could be attributed to other factors not in the dataset.


## Recommendaion
The regression model developed could only account for approximately 57% of variance in house price. 47% is dependent on other unknown variables. Other alternative modelling approaches could be considered.









