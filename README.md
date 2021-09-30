# Udaipur-Rainfall-prediction-using-Time-Series-analysis
In this project we see time series analysis least square method to predict the rainfall in Udaipur district of Rajasthan, India.

# Problem Statement
This study carried out to Udaipur district of Rajasthan. Udaipur receives maximum rainfall due to the south-west monsoon in monsoon season and in all other seasons rainfall is very low for this area. Hence there is always a wide variation in daily annual rainfall as well as seasonal rainfall.

# Objective
Perform time series analysis least square method to predict the rainfall.

# Dataset
Rainfall data:
* Recorded monthly
* Measured in millimeters (mm)
* Starting Date : 01-01-2010
* End Date : 01-12-2020
* district : Udaipur

The dataset taken from knoema https://knoema.com/aulvzxc/district-wise-rainfall-data-for-india?regionId=IN-RJ

# Time series analysis

Time series analysis basically means on the basis of the past we predict future.
In other words understand, interpret and access chronological changes in the value of a variable in the past so that reliable prediction can be made about future value.

We will use least square method for our time series analysis.
During Time Series analysis we come across with variables, many of them are dependent upon others. It is often required to find a relationship between two or more variables.  Least Square is the method for finding the best fit of a set of data points. It minimizes the sum of the residuals of points from the plotted curve. It gives the trend line of best fit to a time series data. This method is most widely used in time series analysis.

Mathematical Representation

The secular trend line (Y) is defined by the following equation:

Y = a + b X

Where, Y = predicted value of the dependent variable

a = Y-axis intercept i.e. the height of the line above origin (when X = 0, Y = a)

b = slope of the line (the rate of change in Y for a given change in X)

When b is positive the slope is upwards, when b is negative, the slope is downwards

X = independent variable (in this case it is time)

To estimate the constants a and b, the following two equations have to be solved simultaneously:

ΣY = na + bΣX

ΣXY = aΣX + bΣX^2

 To simplify the calculations, if the midpoint of the time series is taken as origin, then the negative values in the first half of the series balance out the positive values in the second half so that ΣX = 0. In this case, the above two normal equations will be as follows:

ΣY = na

ΣXY = bΣX^2

In such a case the values of a and b can be calculated as under:

Since ΣY = na

a = ΣY/n

Since, ΣXY = bΣX^2

b = ΣXY/ΣX^2



