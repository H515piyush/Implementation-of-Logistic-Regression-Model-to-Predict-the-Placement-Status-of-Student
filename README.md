# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Import the required packages and print the present data.

2.Print the placement data and salary data.

3.Find the null and duplicate values.

4.Using logistic regression find the predicted values of accuracy , confusion matrices.
Display the results.

## Program:
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.Piyush kumar
Developed by:212223220075 
RegisterNumber:

import pandas as pd
 data=pd.read_csv("C:/Users/admin/OneDrive/Desktop/Placement_Data.csv")
 data.head()
 data1=data.copy
 data1=data.drop(["sl_no","salary"],axis=1)
 data1.head()
 from sklearn.preprocessing import LabelEncoder
 le=LabelEncoder()
 data1["gender"]=le.fit_transform(data1["gender"])
 data1["ssc_b"]=le.fit_transform(data1["ssc_b"])
 data1["hsc_b"]=le.fit_transform(data1["hsc_b"])
 data1["hsc_s"]=le.fit_transform(data1["hsc_s"])
 data1["degree_t"]=le.fit_transform(data1["degree_t"])
 data1["workex"]=le.fit_transform(data1["workex"])
 data1["specialisation"]=le.fit_transform(data1["specialisation"])
 data1["status"]=le.fit_transform(data1["status"])
 data
 x=data1.iloc[:,:-1]
 x
 y=data1["status"]
 y
 from sklearn.model_selection import train_test_split
 x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
 from sklearn.linear_model import LogisticRegression
 lr=LogisticRegression(solver="liblinear")
 lr.fit(x_train,y_train)
 y_pred=lr.predict(x_test)
 y_pred
 from sklearn.metrics import accuracy_score
 accuracy=accuracy_score(y_test,y_pred)
 accuracy
 from sklearn.metrics import classification_report
 classification_report1=classification_report(y_test,y_pred)
 print(classification_report1)
 lr.predict([[1,80,1,90,1,1,90,1,0,85,1,85]])
*/
```

## output:
![Screenshot 2024-03-12 131714](https://github.com/H515piyush/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147472999/95300913-a6ef-4680-896f-0e65dc6ffffc)
![Screenshot 2024-03-12 131722](https://github.com/H515piyush/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147472999/0c3ea778-05fa-4aae-863e-16859154a1b6)



![![Screenshot 2024-03-12 131701](https://github.com/H515piyush/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147472999/f9b8f5c0-87cf-4b1e-bd48-a536f598d03a)
Screensh![Screenshot 2024-03-12 131646](https://github.com/H515piyush/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147472999/9add2638-ab05-44f3-9d19-a9daf927671c)

![Screenshot 2024-03-12 131741](https://github.com/H515piyush/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147472999/d88ad795-2f83-40a7-88a3-c7f05b5c0713)



![Screenshot 2024-03-12 131801](https://github.com/H515piyush/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147472999/0a00e4a5-e3c4-4afa-8216-9d7c99845511)
![Screenshot 2024-03-12 131837](https://github.com/H515piyush/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147472999/fd39b3ba-2cb4-4c67-9ead-d144a015be97)


## Result:

Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
