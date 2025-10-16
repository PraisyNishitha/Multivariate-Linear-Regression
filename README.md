# Implementation of Multivariate Linear Regression
## NAME :PRAISY NISHITHA J
## REFERENCE NO: 212224100042
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1: import panda
<br>

### Step2: import linear model from sklearn
<br>

### Step3:Read the file cars.csv
<br>

### Step4:Assign the value for x and y as required
<br>

### Step5:Create the linear Regression model and predict the output
<br>

## Program:
```

Implementation of Multivariate Linear Regression
Developed by: PRAISY NISHITHA J
RegisterNumber: 212224100042

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients: ',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)




```
## Output:
<img width="618" height="60" alt="443020906-4448ced7-7370-4fe3-b4c7-50a5719b13fc" src="https://github.com/user-attachments/assets/c9a130c9-7c61-4361-b22f-61789bc56ce9" />

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
