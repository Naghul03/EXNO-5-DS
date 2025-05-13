# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

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
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
x=[0,2,4,6,8]
y=[0,10,20,30,40]
plt.plot(x,y,"g*",linestyle="dashed",linewidth=2,markersize=12)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("2D Diagram")
```
![image](https://github.com/user-attachments/assets/3cba5ca4-fd59-492f-9881-27d8336cd223)
```
plt.subplot(2,2,1)
plt.plot(x,y,"r--")
plt.subplot(2,2,2)
plt.plot(y,x,"g*--")
plt.subplot(2,2,3)
plt.plot(x,y,"bo")
plt.subplot(2,2,4)
plt.plot(y,x,"go")
```
![image](https://github.com/user-attachments/assets/cf2f72ae-ecdb-4a14-b056-9048d69cf300)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.plot(x,y)
plt.title("sine wave form")
plt.show()
```
![image](https://github.com/user-attachments/assets/da5aec48-eef2-4d5c-8906-6bfcde4c06eb)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,align="center")
plt.bar(x2,y2,color="g",align="center")
plt.title("Bar Graph")
plt.ylabel("Y-axis")
plt.xlabel("X-axis")
plt.show()
```
![image](https://github.com/user-attachments/assets/4767aa8f-ee1f-44bd-9c19-083f3fe9ac71)
```
x=[1,2,3]
y=[7,3,9]
plt.plot(x,y)
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.title("My First Graph")
plt.show()
```
![image](https://github.com/user-attachments/assets/90ea8c1d-5e10-441f-9549-7dda9fd78df5)
```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel("X axis")
plt.ylabel("Y axis")
plt.title("Two lines")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/a9577b70-6cd4-404f-96b2-7e0c64efc3ac)
```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color="black",linestyle="dashed",linewidth=3,marker="o",markerfacecolor="pink",markersize=12)
plt.xlim(1,8)
plt.ylim(1,8)
plt.xlabel("X axis")
plt.ylabel("Y axis")
plt.title("Customized Plot")
plt.show()
```
![image](https://github.com/user-attachments/assets/bc320d03-6d0b-43a0-9b91-7ddc3e815964)
```
x=[0.895,0.91,0.919,0.926,0.929,0.931]
y=[1,2,3,4,5,6]
plt.plot(x,y)
plt.xlabel("X axis")
plt.ylabel("Y axis")
plt.title("Accuracy")
plt.show()
```
![image](https://github.com/user-attachments/assets/a70bd9aa-3de2-4502-8f6e-b60caf73d96e)
```
apples=[0.91,0.97,0.906,0.94,0.964]
oranges=[0.98,0.93,0.96,0.910,0.973]
years=[2001,2003,2006,2007,2010]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel("Year")
plt.title("crop yeilds in Peru")
plt.legend(["Apples","Oranges"])
```
![image](https://github.com/user-attachments/assets/91e4074a-9d96-4eab-800f-8637bd34260b)
```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker="o")
plt.title("Yeiled of oranges")
```
![image](https://github.com/user-attachments/assets/d293022f-f0a5-400e-805b-0cd476f11109)
```
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker='x')
plt.xlabel("Years")
plt.ylabel("Yeild (tons per hectare)")
plt.title("crop yeilds in Peru")
plt.legend(["Apples", "Oranges"])
```
![image](https://github.com/user-attachments/assets/e9937555-5d99-4569-9208-ec88348a4b8b)
```
import matplotlib.pyplot as plt
x = [1,2,3,4,5,6,7,8,9,10]
y = [2,4,5,6,7,8,9,11,12,13]
plt.scatter(x, y, label="stars", color="green", marker="*", s=30)
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.title("My scatterplot")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/62d683fc-3680-4267-ad02-6ddb9201727a)
```
import matplotlib.pyplot as plt
import numpy as np
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color="orange")
plt.fill_between(x, y2, color="green")
plt.plot(x, y1, color="red")
plt.plot(x, y2, color="black")
plt.legend(["y1", "y2"])
plt.show()
```
![image](https://github.com/user-attachments/assets/3b6a1852-433b-4da3-bc81-1fb5b8f49723)
```
plt.stackplot(x, y1, y2, y3, labels=["line1", "line2", "line3"])
plt.legend(loc="upper left")
plt.title("stacked line chart")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.show()
```
![image](https://github.com/user-attachments/assets/604d71d7-beb3-459d-9c5d-434fcc1f423f)
```
import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x = np.array([1,2,3,4,5,6,7,8,9,10])
y = np.array([2,4,5,7,8,9,10,11,12,13])
spl = make_interp_spline(x, y)
x_smooth = np.linspace(x.min(), x.max(), 100)
y_smooth = spl(x_smooth)
plt.plot(x, y, "o", label="data")
plt.plot(x_smooth, y_smooth, "-", label="spline")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/890a0cdf-50bb-4426-ad91-ed7c5103537c)
```
val=[5,6,7,3,2]
nam=["A","B","C","D","E"]
plt.bar(nam,val)
plt.show()
```
![image](https://github.com/user-attachments/assets/59f3faee-dedf-497b-9fc4-1c6571dc2589)
```
ages = [2, 5, 70, 40, 30, 45, 50, 45, 43, 40, 44, 60, 7, 13, 57, 18, 90, 77, 32, 21, 20, 40]
range = (0, 100)
bins = 10
plt.hist(ages, bins, range, color="purple", histtype="bar", rwidth=0.8)
plt.xlabel("age")
plt.ylabel("No. of people")
plt.title("my histogram")
plt.show()
```
![image](https://github.com/user-attachments/assets/1efb3bc9-48ad-45dd-b67e-b57ead98de2e)
```
x = [2, 1, 6, 4, 2, 4, 8, 9, 4, 2, 4, 10, 6, 5, 7, 7, 3, 2, 7, 5, 3, 5, 9, 2, 1]
plt.hist(x, bins=10, color="violet", alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/2811b2dd-7335-4779-80fe-541ce5cb7afa)
```
np.random.seed(10)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/31b7f61f-c5a8-4618-9d1d-052c8d46f495)
```
fix,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("Data")
ax.set_ylabel("Values")
ax.set_title("Box plot")
```
![image](https://github.com/user-attachments/assets/ad256e41-8d74-4dbe-800b-e5b5c24b1088)
```
activities = ["eat", "sleep", "work", "play"]
slices = [3, 7, 8, 6]
colors = ["r", "y", "g", "b"]
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0, 0.1, 0, 0), autopct="%1.1f%%")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/e61c0557-f399-4ef0-a4d1-4c1b5688f859)
```
labels = 'python', 'C++', 'ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'purple', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True, startangle=140)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/3a56b117-d6ce-40bc-b63c-7848c14b2f9e)

# Result:
 Thus, Data Visualization using matplot python library has been used on the given datas.

