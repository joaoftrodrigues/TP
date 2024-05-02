<img src="https://github.com/joaoftrodrigues/yen-usd-temporal-series-treatment/assets/61411774/28de09f5-7b34-471f-a221-5cf9736884e7" width="500">

# Processing and EDA of time series: Exchange ratio USD/JPY
An application of treatment to a temporal series of exchange rate between JPY (Japanese Yan) and USD (American Dollar), including values imputation and needed
differentiations. The data was extracted from FRED, comprising 20 years, with dates between 1st March, 2003 and 1st March, 2023.

## Context
For an academic project, it's meant to use 3 time series, where 1 is target, and the others are exogenous, to help predict the target one. Each time series 
needed to be treated, to apply further predictions, which was done independently, as for this notebook, is present the treatment on the exogenous variable, 
exchange rate USD/JPY.

## Notes
The project was developed in portuguese, that's the reason all documentation and comments present on the notebook are, at moment, in mentioned language. 
For future, is meant to translate it to english.

One of the time series has monthly data, that's the reason it's applied a transformation on the time frequency of this one, to have all time series in the same
time frequency, such that it can be modelled together. The transformation is done from daily to monthly, for data quality purposes, as it's used known data to do so, while 
the opposite, extrapolation, must predict the values for all different months, leading to scenarios that are not close to the reality, and also it's computationally
more expensive.
