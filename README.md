# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Import the required libraries .

2.Read the data frame using pandas.

3.Get the information regarding the null values present in the dataframe.

4.Apply label encoder to the non-numerical column inoreder to convert into numerical values.

5.Determine training and test data set.

6.Apply decision tree regression on to the dataframe.

7.Get the values of Mean square error, r2 and data prediction.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: PRAISEY S
RegisterNumber: 212222040117
data=pd.read_csv("Salary Data.csv")
data.head()
data.tail()
data.info()
data["Gender"]=data["Gender"].astype('category')
data["Education Level"]=data["Education Level"].astype('category')
data["Job Title"]=data["Job Title"].astype('category')
data.info()
data["Gender"]=data["Gender"].cat.codes
data["Education Level"]=data["Education Level"].cat.codes
data["Job Title"]=data["Job Title"].cat.codes
data.info()
data.head()
x=data[['Age','Gender','Education Level','Job Title','Years of Experience']]
x
x.shape
y=data[['Salary']]
y.shape
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(x, y, test_size=0.2, random_state=2)
from sklearn.tree import DecisionTreeRegressor
dtr=DecisionTreeRegressor()
dtr.fit(x_train,y_train)
y_pred=dtr.predict(x_test)
print(y_pred)
x_train.shape
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dtr.predict([[44,0,2,130,20]])  
*/
```

## Output:

READ CSV HEAD FILE:

![out 7 1](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/f9c77703-56c0-487d-b5e7-650024559e46)

TAIL:

![out 7 2](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/dda5c66b-7a94-42fa-843c-3313cbcc5479)

DATASET INFO:

![out 7 31](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/6986f1e0-1eeb-4719-b969-5ac5db7463be)

![out 7 32](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/235b4fd9-08cc-4ec8-9d1f-17a03f891ff3)

![out 7 33](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/ed341d25-09e4-4623-ba77-c6491ee26387)

![out 7 34](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/86a092d6-7f6e-4ad6-815f-e21881c52b86)

X DATA:

![out 7 4](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/c2f9b2f5-c49a-416a-93bb-013b0e88ef8c)

DATA SHAPE:

![out 7 5](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/f7f59d8d-29d9-43ef-add0-d7f66492c3bf)

Y PRED:

![out 7 6](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/5bfd2ff5-7a26-419d-a8ae-fe4a8d126da3)

MEAN SQUARED VALUE:

![out 7 7](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/a24b7e0a-b628-49af-8b90-284ce4a2fc65)

R2 VALUE:

![out 7 8](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/e5cc412d-b3e6-4a68-a815-387d956b9658)

DTR PREDICT:

![out 7 9](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119394259/5fe54aa0-54eb-47a9-84ad-8e4eb3d9c901)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
