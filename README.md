# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas library.

### Step2
Import Linear_model from sklearn.

### Step3
Read the csv file using pandas library.

### Step4
Enter the parameters of the linear function.

### Step5
Print the parameters of the linear function.

## Program:
```
#program to implement multivariate linear regression and predict the output.
#Developed by : Selvaganesh
#RegisterNumaber : 23012861
import pandas as ps
from sklearn import linear_model
data=ps.read_csv("multi.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predict=regr.predict([[3300,1300]]) 
print('Predicted CO2 for for the corresponding weight and volume',predict)
```
## Output:
![image](https://github.com/etjabajasphin/Multivariate-Linear-Regression/assets/147139861/18ae37db-999b-4609-9264-ccb4845754ed)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
