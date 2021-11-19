# CHEAT SHEET

## Importing different python libraries
### Pandas
```python
import pandas as pd
```
### Matplotlib
```python
import matplotlib.pyplot as plt
```
### Stasmodels.api
```python
import statsmodels.api as sm
```
### Dickey fuller test (adfuller)
```python
from statsmodels.tsa.stattools import adfuller
```
### Autocorrelation function (ACF) and Partial Autocorrelation function (PACF)
```python
from statsmodels.graphics.tsaplots import plot_acf,plot_pacf
```
### ARIMA
```python
from statsmodels.tsa.arima_model import ARIMA
```
### Dateoffset
```python
from pandas.tseries.offsets import DateOffset
```
<br>
<br>

## Reading dataset
```python
df=pd.read_csv('path to your dataset.csv')
```
<br>
<br>

## Cleaning dataset
![image](https://user-images.githubusercontent.com/52816788/142578681-c00b27fe-e7e6-41f2-a6a4-2cfdafbba15c.png)

For eg. here as you can see in the above image the columns with the index 0, 1, 2 and 3 data were not wanted for our analysis so we used the following syntax to remove it:
### For columns:
```python
df.drop(df.columns[[column index numbers seperated by commas]], axis = 1, inplace = True)
```
### For rows:
```python
df.drop(df.rows[[rows index numbers seperated by commas]], axis = 0, inplace = True)
```

The above two syntaxs are used to remove unwanted or nan data from our dataset.

<br>
<br>

## How to calculate p, d and q order for the arima model
To calculate the p value we make PACF graph and the point where the sudden shutdown or decrease happens.
![image](https://user-images.githubusercontent.com/52816788/142607886-f96902f9-2c22-43d5-9221-43136323e81d.png)

For eg. look at the above figure after 2 points sudden decrease happens so p value will be 2.
<br>
To d value is equal to number of time differencing has been done.
<br>
To find the q value we see the ACF graph and select any value between 0 and the point where graph looks like it is decreasing exponentially all works fine.
![image](https://user-images.githubusercontent.com/52816788/142609319-12c99f67-079b-45a5-aa58-f382c321c23b.png)
for eg. lets see the above figure as you can see we can say graph is decreasing exponentially till 6th point so the q value can either be 0, 1, 2, 3, 4, 5 or 6.

