# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.
### Step2
Read the CSV file.
### Step3
Get the value of x and y variables.
### Step4
Create the linear regression model and fit.
### Step5
Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3.
### step6
Print the predicted output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)

```
## Output:
![Screenshot (85)](https://github.com/Pradeeppachiyappan/Multivariate-Linear-Regression/assets/118707347/60af19c6-b46c-42ff-b382-b2c5276512d7)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
