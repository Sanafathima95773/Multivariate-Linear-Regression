# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
import pandas module to solve for multivariate linear regression

### Step2
<br>
from sklearn import linear_model

### Step3
<br>
open the file cars saved in drive and get input for weight and volume to find density of CO2

### Step4
<br>
print coefficients,intercept and amount

### Step5
<br>
End of program

## Program:
```
#implemetation of multivariate linear regression
#Developed by: Sana Fathima H
#Register number: 212223240145
import pandas as pd
from sklearn import linear_model
df=pd.read_csv('/content/drive/My Drive/cars (1).csv')
x=df[['Weight','Volume']]
y=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))

```
## Output:
![alt text](<Screenshot 2024-05-08 093600.png>)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.