# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.import numberical python

2.import sys

3.give the input

4.type the required functions


## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: NAVEEN KUMAR.B
RegisterNumber: 212222230091 
import numpy as np
import sys
n=int(input())
a = np.zeros((n,n+1))
x = np.zeros(n)

for i in range(n):
    for j in range(n+1):
        a[i][j]= float(input())
        
for i in range(n):
    if a[i][j]==0.0:
            sys.exit('Divide by zero detected!')
            
    for j in range(i+1,n):
        ratio = a[j][i]/a[i][i]
        
        for k in range(n+1):   
                a[j][k] = a[j][k] - ratio*a[i][k]    

x[n-1]= a[n-1][n]/a[n-1][n-1]

for i in range(n-2,-1,-1):
    x[i]=a[i][n]
    
    for j in range(i+1,n):
       x[i] = x[i]-a[i][j]*x[j]
       
    x[i] = x[i]/a[i][i]
    
for i in range(n):
    print('X%d = %0.2f' %(i,x[i]),end=' ') 
*/
```

## Output:
![image](https://github.com/mrnaviz/Gaussian/assets/123350791/3828ea47-fed7-465d-b63d-e980ae4b5158)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

