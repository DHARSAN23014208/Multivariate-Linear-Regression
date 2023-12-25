# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.
### Step3
Get the value of X and y variables.
### Step4
Create the linear regression model and fit.
### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3.

## Program:
```
Developed by:DHARSANKUMAR R
Register number:23014208
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars (1).csv")
x=df[['Weight','Volume']]
Y=df['co2']
regr=linear_model.linearRegression()
regr.fit(X,Y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedco2=regr.predict([[3300,1300]])
print('predicted co2 for the corresponding weight and volume',predictedco2)

```
## Output:
![image](https://github.com/DHARSAN23014208/Multivariate-Linear-Regression/assets/149365413/9b3d8607-0b9c-4b30-90fb-b3d6c45ea11a)

### Insert your output



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
