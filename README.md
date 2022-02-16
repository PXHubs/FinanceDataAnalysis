# Financial Stock Data Project
The purpose of this project to evaluate the stock data on major banks, Goldman Sachs, Bank of America, Citigroup, JP Morgan, Morgan Stanley, and Wells Fargo. The focus is on exploratory data analysis of those bank stock prices using visualization and pandas in python. The data will be primarily be in 4 year period from 2018 to 2022. 

# Extracting data and Consolidate
The first step is to establish all of the import modules that are needed for the data analysis as well as determining a date.time value for start to end date. Using DataReader from pandas and therefore yahoo, all the banks stock data are extracted. Then a list is created for naming of the banks for all the columns in concatenation process using pandas dataframe. The end results are as follows. 

Using the cross sheet method, the function can key in the column(axis=1) 'Close' in the dataframe on stock info row or level in this case. The highest value was extracted from each of the banks and the output were as follows.

BAC     49.380001
C       81.910004
GS     423.850006
JPM    171.779999
MS     108.730003
WFC     59.060001

