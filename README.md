# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the required libraries, such as pandas and linear_model from sklearn.

### Step2
Load the dataset using pd.read_csv() function, specifying the correct file path.

### Step3
Extract the features and target variable from the dataset.

### Step4
Create a linear regression model object using linear_model.LinearRegression() and train the model using fit() method.

### Step5
Use the trained model to predict CO2 emissions for a given weight and volume using predict() method.

## Program:
```
import pandas as pd
from sklearn import linear_model
data=pd.read_csv("car.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficients:",regr.coef_)
print("Intercept:",regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for corresponding weight and volume",predictCO2)
```
## Output:

![image](https://github.com/Visalan-H/Multivariate-Linear-Regression/assets/152077751/5093b5d4-2621-4584-ab76-698fcd65efad)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
