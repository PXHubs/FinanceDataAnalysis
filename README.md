# Financial Stock Data Project
The purpose of this project to evaluate the stock data on major banks, Goldman Sachs, Bank of America, Citigroup, JP Morgan, Morgan Stanley, and Wells Fargo. The focus is on exploratory data analysis of those bank stock prices using visualization and pandas in python. The data will be primarily be in 4 year period from 2018 to 2022. 

# Extracting data and Consolidate
The first step is to establish all of the import modules that are needed for the data analysis as well as determining a date.time value for start to end date. Using DataReader from pandas and therefore yahoo, all the banks stock data are extracted. Then a list is created for naming of the banks for all the columns in concatenation process using pandas dataframe. The end results are as follows. 

![image](https://user-images.githubusercontent.com/98336842/154355024-07a84ab1-f425-4e64-899b-8be822bec03f.png)


Using the cross sheet method, the function can key in the column(axis=1) 'Close' in the dataframe on stock info row or level in this case. The highest value was extracted from each of the banks and the output were as follows.

![image](https://user-images.githubusercontent.com/98336842/154355150-6fc20c36-6a31-483f-b3aa-a1e45c1602a1.png)


# Retreiving Returns
In order to calculate the returns on a daily basis on each of the bank stocks, an empty dataframe is called and then provide a function. The for loop is as follows: for the elements in tickers such as BAC, C, or GS, apply the pct.change() function to each individual stocks under the new name 'tick'+'Return'. The function Bank_stocks[tick]['Close'] provides the multi-level column where the tick mentioned will return the 'close' column. This for loop is reiterated for all of the banks mentioned and at the end, the result is the following:  

![image](https://user-images.githubusercontent.com/98336842/154357053-ad007d75-5d0a-441b-8ffe-985ca275ca6b.png)

#Statistics 
Using idx method where it returns the index of the first occurance that happens, the minimum and maximum returns are located. All the dates revolves around March of 2020, the global pandemic started. Standard deviation and histograms of all banks are calculated.

We then plotted all of the pricing an interactive plot using iplot as well as plotting the moving averages of all of the banks. The heat maps are then created for any type of correlation that happens. 

![image](https://user-images.githubusercontent.com/98336842/154366744-96e658f0-27ed-43dd-96f2-6a6ced61423b.png)


![image](https://user-images.githubusercontent.com/98336842/154366663-bf712de5-2517-4a25-b9b1-be399bfa63a9.png)
