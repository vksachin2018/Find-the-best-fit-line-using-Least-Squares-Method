# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start
2. Get the independent variable X and dependent variable Y.
3. Calculate the mean of the X -values and the mean of the Y -values.
4. Find the slope m of the line of best fit using the formula.
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
 5. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
 6. Use the slope m and the y -intercept to form the equation of the line.
 7. Obtain the straight line equation Y=mX+b and plot the scatterplot.
 8. Stop

## Program:
```
Developed by
Name :Gokul sachin
Reg no: 212223220025
```
```
import numpy as np
import matplotlib.pyplot as plt
X = np.array(eval(input()))
Y = np.array(eval(input()))
X_mean = np.mean(X)
Y_mean = np.mean(Y)
num = 0
denom=0
for i in range(len(X)):
  num+=(X[i] - X_mean)*(Y[i]-Y_mean)
  denom+=(X[i]-X_mean)**2
m = num/denom
b = Y_mean - m*X_mean
print(m,b)
y_predicted = m*X + b
print(y_predicted)
plt.scatter(X,Y)
plt.plot(X,y_predicted,color='red')
plt.show()
```

## Output:
![image](https://github.com/arbasil05/Find-the-best-fit-line-using-Least-Squares-Method/assets/144218037/83c08f4e-65b2-4cc7-b1d5-b778dee55012)


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
