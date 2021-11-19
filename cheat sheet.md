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

## Cleaning dataset
![image](https://user-images.githubusercontent.com/52816788/142578681-c00b27fe-e7e6-41f2-a6a4-2cfdafbba15c.png)

For eg. here as you can see in the above image the columns with the index 0, 1, 2 and 3 data were not usefull for our analysis so we used the following syntax to remove it:
### For columns:
```python
df.drop(df.columns[[column index numbers seperated by commas]], axis = 1, inplace = True)
```
