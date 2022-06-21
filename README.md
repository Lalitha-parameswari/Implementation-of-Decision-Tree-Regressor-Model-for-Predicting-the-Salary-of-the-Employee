# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the standard libraries.
2. Upload the dataset and check for any null values using .isnull() function.
3. Import LabelEncoder and encode the dataset.
4. Import DecisionTreeRegressor from sklearn and apply the model on the dataset.
5. Predict the values of arrays.
6. Import metrics from sklearn and calculate the MSE and R2 of the model on the dataset.
7. Predict the values of array.
8. Apply to new unknown values.
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: LALITHA PARAMESWARI.C
RegisterNumber:212219220027
import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:

## Data Head:

![image](https://user-images.githubusercontent.com/103946827/174736420-63e6a303-80f1-4921-821e-f0178cc4f67e.png)

## Data Info:

![image](https://user-images.githubusercontent.com/103946827/174736492-bd3fd9ec-f34c-4cdf-9c99-5ea94a6fa0cc.png)

## Data Isnull:

![image](https://user-images.githubusercontent.com/103946827/174736577-ddbeccfe-100d-48d9-baaa-6db0e7c15a39.png)

## Data Head:

![image](https://user-images.githubusercontent.com/103946827/174736641-19c43807-0f73-465c-bf81-6585c97b3057.png)

## MSE:

![image](https://user-images.githubusercontent.com/103946827/174736707-4c4cd78d-87e8-47b0-8449-7f7b07b8920b.png)

## R2:

![image](https://user-images.githubusercontent.com/103946827/174736770-615da9e8-b7d0-449d-96d7-c054b7aaf665.png)

## Predicted Value:

![image](https://user-images.githubusercontent.com/103946827/174736824-003749db-a12f-4094-8b2e-8b371dd40d6d.png)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
