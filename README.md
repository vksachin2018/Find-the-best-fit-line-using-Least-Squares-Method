# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
STEP 1 START

STEP 2: Get the independent variable X and dependent variable Y.

STEP 3: Calculate the mean of the X -values and the mean of the Y -values.

STEP 4: Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">

STEP 5:Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">

STEP 6:Use the slope m and the y -intercept to form the equation of the line.

STEP 7: Obtain the straight line equation Y=mX+b and plot the scatterplot.

STEP 8 STOP
## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: gokul sachin k
RegisterNumber: 212223220025
import numpy as np
import matplotlib.pyplot as plt

X = np.array(eval(input()))
Y = np.array(eval(input()))

X_mean=np.mean(X)
Y_mean=np.mean(Y)

num = 0
denom = 0

for i in range(len(X)):
    num += (X[i]-X_mean)*(Y[i]-Y_mean)
    denom += (X[i]-X_mean)**2

m = num/denom

b = Y_mean - m*X_mean
print (m, b)


Y_pred = m*X+b
print (Y_pred)


print("X values : ",X)
print("Y values : ",Y)
dots=[150]
plt.figure(figsize=(10, 8))
plt.scatter(X,Y,color='green',s=dots)
plt.plot(X,Y_pred,color='red',linewidth=4)
plt.xlabel("X-axis",fontweight='bold',fontsize=20)
plt.ylabel("Y-axis",fontweight='bold',fontsize=20)
plt.show()


```

## Output:
![best fit line]
![309690930-9c2ab1bd-37d3-4ea1-b2f5-6cc2c1fbf9f7](https://github.com/vksachin2018/Find-the-best-fit-line-using-Least-Squares-Method/assets/149366019/98e7cf46-2236-414d-8f82-0ed698f255cd)

## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
