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
RegisterNumber: 212224230293

import pandas as pd
from google.colab import files
uploaded = files.upload()
data= pd.read_csv('/content/Employee.csv')
data.head(10)

data.info()
data.isnull().sum()
data['left'].value_counts()

from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()

data['salary'] = le.fit_transform(data['salary'])
data.head()

x=data[['satisfaction_level','last_evaluation','number_project','average_montly_hours','time_spend_company','Work_accident','promotion_last_5years','salary']]
x.head()

y=data['left']

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state =100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion='entropy')
dt.fit(x_train,y_train)
y_predict=dt.predict(x_test)


from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_predict)
accuracy


dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:

![Screenshot 2025-04-23 105207](https://github.com/user-attachments/assets/0b7c561f-0f5c-41a0-addc-9a8bbcbf5ab0)

![Screenshot 2025-04-23 105313](https://github.com/user-attachments/assets/d550de4d-bfe9-46ac-8e99-6a56e55cc7f3)

![Screenshot 2025-04-23 105351](https://github.com/user-attachments/assets/f24c1ade-c9e5-4e51-8382-756215d55a66)

![Screenshot 2025-04-23 105453](https://github.com/user-attachments/assets/a899aa43-e0e2-436c-8ae7-927000b2f4de)

![Screenshot 2025-04-23 105626](https://github.com/user-attachments/assets/6163d569-bb97-40e8-8267-95dbcfd98410)

![Screenshot 2025-04-23 105646](https://github.com/user-attachments/assets/885405fb-b853-4b23-9265-c50e63880f84)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
