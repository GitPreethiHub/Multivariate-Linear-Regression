# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import panda module as pd

### Step2
<br>Import linear model from sklearn

### Step3
<br>Read the file cars.csv

### Step4
<br>Assign the values for x and y as required

### Step5
<br>Create the linearRegression model and predict the output

## Program:
```
'''
Developed by: Preethi M
Register number: 212222100037
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:

![image](https://github.com/GitPreethiHub/Multivariate-Linear-Regression/assets/119475585/0ccb2e0e-589e-4016-8a5a-2b4651c736a9)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
