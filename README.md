# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: N.PRAVESH
RegisterNumber:  212223230154
x = eval(input())
y = eval(input())
n = len(x)
xbar = sum(x)/n
ybar = sum(y)/n
x_min_xbar = []
y_min_ybar = []
prod_xy = []
x_min_xbar_sq = []

for i in range(n):
  x_min_xbar.append(x[i] - xbar)
  y_min_ybar.append(y[i] - ybar)
  prod_xy.append(x_min_xbar[i]*y_min_ybar[i])
  x_min_xbar_sq.append(x_min_xbar[i]**2)
s_xy = sum(prod_xy)
s_x_min_xbar_sq = sum(x_min_xbar_sq)
m = s_xy/s_x_min_xbar_sq
c = ybar - m*xbar
print(f"m = {round(m,2)}")
print(f"c = {round(c,2)}")
print(f"Y = {round(m,2)}x + {round(c,2)}")

*/
```

## Output:
![Screenshot 2024-08-20 132058](https://github.com/user-attachments/assets/7e4f91d6-f451-45ca-ae11-43249fc465ec)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
