# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries.
2. Upload the csv file and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree inport DecisionTreeRegressor.
5. Import metrics and calculate the Mean squared error.
6. Apply metrics to the dataset, and predict the output. 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: MUHAMMED ASHIQ B
RegisterNumber: 212220040094

import pandas as pd
data = pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["Position"] = le.fit_transform(data["Position"])
data.head()
x = data[["Position","Level"]]
y = data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_pred)
mse
r2 = metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
![11](https://user-images.githubusercontent.com/104640895/173218010-7b339295-0674-4c93-9ba4-d1bc50301a04.png)
![22](https://user-images.githubusercontent.com/104640895/173218057-117be7f3-c8f6-42a9-a451-e0bc3857f196.png)
![33](https://user-images.githubusercontent.com/104640895/173218068-8dce93a6-901e-491c-ab6e-61be28cff6ff.png)
![44](https://user-images.githubusercontent.com/104640895/173218077-ea99ab71-31dd-4c88-b9f2-c90a9cbe3d00.png)
![55](https://user-images.githubusercontent.com/104640895/173218082-372e6b46-07ac-410a-8a81-4e481f68ea80.png)
![66](https://user-images.githubusercontent.com/104640895/173218089-702cf781-cb20-4a6e-a169-870ae8c66ea5.png)
![77](https://user-images.githubusercontent.com/104640895/173218096-c2cd2f2b-02a8-4a4a-9b5b-4a55b42b6c21.png)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
