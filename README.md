# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the packages.

2.Analyse the data.

3.Use modelselection and Countvectorizer to preditct the values.

4.Find the accuracy and display the result.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: E Hemachandran
RegisterNumber: 212224230093

import chardet
file="spam.csv"
with open(file, 'rb') as rawdata:
    result = chardet.detect(rawdata.read(100000))
result
import pandas as pd
data=pd.read_csv("spam.csv",encoding='Windows-1252')
data.head()
data.isnull().sum()
data.info()
x=data["v2"].values
y=data["v1"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
x_train
from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()
x_train = cv.fit_transform(x_train)
x_test = cv.transform(x_test)
x_train
x_test
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
conf=metrics.confusion_matrix(y_test,y_pred)
conf
print("E Hemachandran")
print("212224230093")
c=metrics.classification_report(y_test,y_pred)
c
*/
```

## Output:


<img width="772" height="40" alt="image" src="https://github.com/user-attachments/assets/86ab21b9-8c8f-4ffb-8649-5db49dce5d44" />


<img width="862" height="248" alt="image" src="https://github.com/user-attachments/assets/b6ec8f9e-d4b6-457f-bd9e-61630a8ffe17" />


<img width="240" height="145" alt="image" src="https://github.com/user-attachments/assets/b373cdcb-5442-40bd-91af-4df1b9a36881" />


<img width="388" height="267" alt="image" src="https://github.com/user-attachments/assets/2b8fe1d4-d6bb-4516-8a7d-5e851551b3cc" />


<img width="888" height="252" alt="image" src="https://github.com/user-attachments/assets/4383d81e-66a8-4517-8d76-368f307f56a0" />


<img width="661" height="206" alt="image" src="https://github.com/user-attachments/assets/a5e75d0b-80ac-4c76-84b9-673614d774f4" />


<img width="907" height="161" alt="image" src="https://github.com/user-attachments/assets/b04c5d81-ff8a-4361-bcd3-a680139fb82c" />


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
