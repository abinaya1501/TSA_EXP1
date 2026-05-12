# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 22.04.2026
# AIM:
#### Dataset: Video_Games_Sales
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
from matplotlib import pyplot as plt
import pandas as pd

df = pd.read_csv("/content/Video_Games_Sales.csv")

print(df.head())

print(df.dtypes)

plt.title('Time Series Plot of Video Game Global Sales')
plt.xlabel('Year')
plt.ylabel('Global Sales (Millions)')

plt.plot(df['Year_of_Release'], df['Global_Sales'], label = 'Global Sales')
plt.legend()
plt.grid(True)
plt.show()
```
# OUTPUT:

<img width="704" height="518" alt="Screenshot 2026-04-22 111124" src="https://github.com/user-attachments/assets/58b71534-46e2-4a9d-a040-407a99881368" />
# RESULT:
Thus we have created the python code for plotting the time series of given data.
