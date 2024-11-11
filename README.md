EX 05 : DS
# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line 1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two line on same graph')
plt.legend()
```
![image](https://github.com/user-attachments/assets/71288043-0655-4454-a58b-c796bc122e9a)

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('some cool customization')
```
![image](https://github.com/user-attachments/assets/6eb25b72-a1eb-4e8f-afd7-3d6ff4f071a5)
```
years = range(2000, 2012)
apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.903, 0.907, 0.904, 0.901, 0.896, 0.896]

plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')

plt.title("Crop Yields in Kanto")
plt.legend(['Apples', 'Oranges'])
```
![image](https://github.com/user-attachments/assets/985d5b30-04af-45d6-83d5-507240b198d2)
```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="blue")
plt.show()
```
![image](https://github.com/user-attachments/assets/a7401c5d-f166-4012-b75c-003503926f47)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label="stars",color="green",marker="*",s=30)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("Scatter Plot")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/b70ff6a4-2f6f-49da-bc13-6e979cac6e36)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![image](https://github.com/user-attachments/assets/dfc889c8-b3dd-4a7f-a397-a75c5a922af8)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("2d Diagram")
plt.show()
```
![image](https://github.com/user-attachments/assets/d64fc8ee-933f-4b0d-a6eb-7cc27ffb4bda)

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
![image](https://github.com/user-attachments/assets/46d90dcc-bf02-4024-a541-30bdd98f9660)

```
import numpy as np
import matplotlib.pyplot as plt
x = np.arange(0, 4 * np.pi, 0.1)
y = np.sin(x)
plt.title("Sine Wave Form")
plt.plot(x, y)
plt.show()
```
![image](https://github.com/user-attachments/assets/8996be3d-79db-4f50-87e4-d60921db49d0)

```
import matplotlib.pyplot as plt
import numpy as np

# Create some random data
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]

# Create the plot
plt.fill_between(x, y1, color='pink')
plt.fill_between(x, y2, color='yellow')

plt.plot(x, y1, color='violet')
plt.plot(x, y2, color='orange')

plt.legend(['y1', 'y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/5533b200-7378-46ed-a5c8-c8271df2859f)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['pink','yellow']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/0e281e7a-a9be-4d48-8ce5-8044400a2651)

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='pink')
plt.bar(x2,y2,color='yellow')
plt.xlabel('x - axis')
plt.ylabel('y - axis')

plt.show()
```
![image](https://github.com/user-attachments/assets/4b3fc92e-41ac-4307-a7f1-285bd918f555)
```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='pink',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('age distribution')
plt.show()
```
![image](https://github.com/user-attachments/assets/6066333a-055e-4401-9958-017c8a40ccc3)

![image](https://github.com/user-attachments/assets/4438d4a5-99c7-44fd-ba25-9886db0ca402)

![image](https://github.com/user-attachments/assets/5fba1544-b6bb-48e3-9269-007d9c822916)
![image](https://github.com/user-attachments/assets/a0cb2c99-cb66-4a67-ba6d-e9d3ef80b376)
![image](https://github.com/user-attachments/assets/a13938c0-fdbc-443c-934f-3775d3c9d423)
![image](https://github.com/user-attachments/assets/ff7e2e4c-319e-40d8-8c6b-4f4d5db43adb)

# Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
