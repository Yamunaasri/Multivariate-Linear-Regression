# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Read the given dataset.
<br>

### Step2
Assign the attributes to X and Y respectively.
<br>

### Step3
Fit the X and Y features.
<br>

### Step4
Apply the Linear Regression Model to find the coefficient and intercept.
<br>

### Step5
Calculate the Prediction for CO2.
<br>

## Program:
```

import pandas as pd
from sklearn import linear_model
df= pd.read_csv("/content/cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient",regr.coef_)
print("Intercept",regr.intercept_)
predictionCO2=regr.predict([[3300,1300]])
print("Prediction CO2 for the corresponding weight and volume",predictionCO2)


```
## Output:

Coefficient [0.00755095 0.00780526]
Intercept 79.69471929115939
Prediction CO2 for the corresponding weight and volume [114.75968007]



### Insert your output
![Screenshot 2023-05-29 144440](https://github.com/Yamunaasri/Multivariate-Linear-Regression/assets/115707860/6da0a451-adfd-4923-bce6-359dd0daf725)
<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
