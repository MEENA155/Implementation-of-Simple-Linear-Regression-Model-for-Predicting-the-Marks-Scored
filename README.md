# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to implement the simple linear regression model for predicting the marks scored.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
1.For Gradient Design use the standard libraries in the python.
2.Use the .isnull()function to check the empty .
3.Use the default function.
4.Use the loop function for a linear equation.
5.Predict the value for the y.
6.Print the program.
7.plot the graph by using scatters keyword.
8.End the program
```

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: S.Meena
RegisterNumber: 212221240028
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv("/content/student_scores - student_scores.csv")
data.head()
data.isnull().sum()
x=data.Hours
x.head()
y=data.Scores
y.head()
n=len(x)
m=0
c=0
l=0.001
loss=[]
for i in range(10000):
    ypred=m*x+c
    MSE=(1/n)*sum((ypred-y)*2)
    dm=(2/n)*sum(x*(ypred-y))
    dc=(2/n)*sum(ypred-y)
    c=c-l*dc
    m=m-l*dm
    loss.append(MSE)
    #print(m,c)
    ypred=m*x+c
plt.scatter(x,y,color="purple")
plt.plot(x,ypred)
plt.xlabel("study hours")
plt.ylabel("scores")
plt.title("study hour vs scores")
plt.plot(loss)
plt.xlabel("iteration")
plt.ylabel("loss")
*/
```

## Output:
![Screenshot (21)](https://user-images.githubusercontent.com/94677128/162013965-abd76c6b-61e4-40a2-b6ab-4fa5be758aeb.png)
![Screenshot (22)](https://user-images.githubusercontent.com/94677128/162014196-e7d94897-b009-4231-9057-a733c83fbf8b.png)



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
