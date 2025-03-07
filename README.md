# Ex.No: 1A PLOT A TIME SERIES DATA
## DATE : 04/03/2025

## AIM :
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.

## ALGORITHM :
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
   
## PROGRAM :
```
Developed By: NITHYA D
Reg.no: 212223240110
```
```
import pandas as pd
import matplotlib.pyplot as plt
file_path = 'Gold Price Prediction.csv'
data = pd.read_csv(file_path)
data['Date'] = pd.to_datetime(data['Date'])
data.set_index('Date', inplace=True)
plt.figure(figsize=(10, 6))
plt.plot(data.index, data['Price Today'], label='Gold Price Today', color='gold')
plt.title('Gold Price Today Over Time')
plt.xlabel('Date')
plt.ylabel('Gold Price')
plt.grid(True)
plt.legend()
plt.show()
```

## OUTPUT :
![image](https://github.com/user-attachments/assets/33d25dfa-0db9-4ebe-9448-f3c510f72c3b)

## RESULT :
Thus we have created the python code for plotting the time series of given data.
