# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 24 . 04. 2026
## Name : ABINAYA A
## Reg no : 212224230004
# AIM:
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
import pandas as pd
import matplotlib.pyplot as plt

# Load the CSV file
file_path = 'Gold Price Prediction.csv'  # Replace with your file path
data = pd.read_csv(file_path)

# Convert 'Date' column to datetime format
data['Date'] = pd.to_datetime(data['Date'])

# Set 'Date' as the index
data.set_index('Date', inplace=True)

# Plot the time series of 'Price Today'
plt.figure(figsize=(10, 6))
plt.plot(data.index, data['Price Today'], label='Gold Price Today', color='blue')

# Customize the plot
plt.title('Gold Price Today Over Time')
plt.xlabel('Date')
plt.ylabel('Gold Price')
plt.grid(True)
plt.legend()

# Display the plot
plt.show()


```








# OUTPUT:
<img width="1252" height="728" alt="image" src="https://github.com/user-attachments/assets/67d9de4d-78f3-40f6-a4cd-ee241c0a226c" />






# RESULT:
Thus we have created the python code for plotting the time series of given data.
