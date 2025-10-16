# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the required libraries such as pandas and linear_model from sklearn for data handling and regression analysis.
<br>

### Step2
Read the dataset “car_data.csv” using pandas and store it in a DataFrame.
<br>

### Step3
Select the independent variables Volume and Weight as input features (x) and CO2 as the target variable (y).
<br>

### Step4
Create a Linear Regression model using sklearn and fit it with the input and output data.
<br>

### Step5
Display the coefficients and intercept of the model, and make a prediction for given input values.
<br>

## Program:

```
#Name: A Ahil Santo
#Reg No: 212224040018
import pandas as pd
from sklearn import linear_model
df=pd.read_csv(r"E:\Desktop\CSE\Maths for AI\car_data.csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
reg=linear_model.LinearRegression()
reg.fit(x,y)
print("Coefficient: ",reg.coef_)
print("Intercept: ",reg.intercept_)
pred=reg.predict([[3300,1300]])
print("Prediction: ",pred)
```
## Output:

<img width="774" height="411" alt="image" src="https://github.com/user-attachments/assets/7240f211-0804-43fe-8223-cf05c7d2e9e4" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
