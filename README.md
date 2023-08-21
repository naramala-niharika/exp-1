# EXP-1-Plot-a-time-series-data

## AIM:
###  Develop a python program to Plot a time series data (population/ market price of a commodity /temperature.

## ALGORITHM:
### STEP 1: Import the required packages like pandas and numpy
### STEP 2: Read the data using the pandas
### STEP 3: Calculate the mean for the respective column.
### STEP 4: Plot the data according to need and can be altered monthly, or yearly.
### STEP 5: Display the results.

## PROGRAM:
```
import matplotlib.pyplot as plt
import pandas as pd
df=pd.read_csv("Dataset.csv",parse_dates=["Date"],index_col="Date")
df.head()
df["2022-01"]
df["2022-01"].Close.mean()
df["2022-04-01":"2022-07-31"]
df.Close.resample('M').mean()
mean=df.Close.resample('M').mean().plot(kind="bar")
mean=df.Close.resample('Y').mean().plot(kind="bar")
```

## OUTPUT:

### FIRST FIVE ROWS:

![261806643-966e903b-c051-4846-bf0a-278477394d6a](https://github.com/naramala-niharika/exp-1/assets/94165377/af7ed561-edc4-4083-9c24-ac455488f89f)

### CALCULATING MEAN:
![261806659-952c90de-b90f-4000-8075-4c973d13bc0e](https://github.com/naramala-niharika/exp-1/assets/94165377/0c83e690-af74-4500-a99f-b72bf98b30c6)


### PLOTTING BAR GRAPH(MONTHLY):
![261806670-db848b6d-d98d-4f87-829b-d2ba877a3afc](https://github.com/naramala-niharika/exp-1/assets/94165377/d29adcfc-edcb-452d-8631-b482a6206c62)


### PLOTING BAR GRAPH(YEARLY):

![261806698-16f7788b-75ec-4dfa-b2b5-80db53d52a09](https://github.com/naramala-niharika/exp-1/assets/94165377/3a100659-ebb6-4ae1-a0e0-6db5a42d77a8)

## RESULT:
### Thus we have created the python code for plotting the time series of given data.
