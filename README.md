# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:

1. Import pandas
2. Import Decision tree classifier
3. Fit the data in the model
4. Find the accuracy score



## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: TRISHA PRIYADARSHNI PARIDA
RegisterNumber:  212224230293


import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]]) 
*/
```

## Output:

![Screenshot 2025-04-23 105207](https://github.com/user-attachments/assets/28670c2e-5706-4953-8a7f-4e9a8483c8fc)

![Screenshot 2025-04-23 105313](https://github.com/user-attachments/assets/c446cdb5-31b7-4f61-b6f4-8c7930b23dd5)

![Screenshot 2025-04-23 105351](https://github.com/user-attachments/assets/61258733-8f2c-4c7b-8b90-dd07cc2c1f3e)

![Screenshot 2025-04-23 105453](https://github.com/user-attachments/assets/37050fa3-db59-4f27-8037-51fbd395ad66)

![Screenshot 2025-04-23 105626](https://github.com/user-attachments/assets/1c1347d3-4534-4c3c-b201-7f0b39ce212b)

![Screenshot 2025-04-23 105646](https://github.com/user-attachments/assets/131b0329-e89d-4375-a1ba-c25f622de077)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
