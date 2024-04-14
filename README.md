# 6150 Final Project
## Introduction:
### Purpose:
The main objective for this analysis is to identify trends within the history of Starbucks stocks prices. Specifically, to locate all time high and low prices, high and low averages, and possible trends throughout the years. 

### More about Starbucks: 
This coffee company was founded in Seattle Washington in 1971. Starbucks is known for their high-quality coffee beans and have over 87,000 different possible coffee combinations. Although, they do provide a variety of drinks such as matcha, tea, flavored refreshers, and more. Starbucks has over 36,000 locations around the world, although they did not begin this way. This analysis will focus on identifying the highs and lows of this company. 

## Selection of data:
The data was switched to the stocks history of Starbucks in order to analyze a familiar company. 

https://www.nasdaq.com/market-activity/stocks/sbux/historical

### Starbucks Stock History Dataset: 
The dataset was sourced from the Nasdaq website. Nasdaq or the National Association of Securities Dealers Automated Quotations was founded in New York City, New York, in 1971. Nasdaq is a reliable source, as it was the first company to bring the stock market to the internet. This company provides daily stock data for many companies.

### Characteristics of data: 
This dataset provides the stock history for Starbucks from 2014 to 2020. It includes columns identifying the date, close price, volume, open price, high price, and low price. 

### Data Preparation: 
The data was revised to proceed with a smooth analysis. First, the “$” was removed from the data to ensure the code would properly return the correct output. For example, this code exemplifies how the “$” was removed from the high column and turned into a float. 

![Panda-Revision](/graph/Picture1.png)

Next, the date column was turned into a datetime using Pandas, in order to easily navigate the dates.  

![Panda-Datetime](/graph/Picture2.png)

As a result, the data should have disregarded the “$” within the rows, and the dates have transformed into the datetime format. This dataset has 6 columns and 1691 rows.  

![Data-Preview](/graph/Picture3.png)

There were no missing values in the data therefore, no imputations. In addition, there was no feature engineering, although this analysis utilized the cleaned data in order to find the answers to the three questions. 

## Methods: 

### Tools: 
-Pandas

-Matplotlib 

-Seaborn

### Pandas: 
In this analysis, pandas was used to read, clean, and to conduct statistical testing on the data. 
‘pd.read_csv()’ was used in order to efficiently load the dataset. 

![Data](/graph/Picture4.png)

The pandas library allowed for the removal of the “$”. In addition to the conversion of the data from string to float. 

![Data](/graph/Picture5.png)

Also, pandas was helpful in order to conduct statistical testing. Such as finding the maximum value within a column. 

![Data](/graph/Picture6.png)

### Matplotlib: 
Matplotlib was used to visualize the trends in the data by making a plot. In this example, ‘plt.plot’ was used in order to create a plot of the high and low data over time. 

![Data](/graph/Picture7.png)

### Seaborn: 
Seaborn was used to visualize the highest monthly average prices per year. In this example, ‘sns.barplot’ was used in order to create a boxplot. 

![Data](/graph/Picture8.png)

## Results: 

### Question 1: When did the price of the stock reach a high? When did it reach a low? 

First, graphs were created to visualize the stock trends. The stock prices somewhat have a positive trend. Although, there was a significant drop in 2020. 

![Data](/graph/Picture9.png)

The high and low prices were identified for each column. 

![Data](/graph/Picture10.png)

Based on all this data, the stock reached a high on December 10th, 2020 at a price of $106.09. The stock reached a low on April 11th, 2014. 

### Question 2: Which year did the stock price have the highest average? The lowest average?

![Data](/graph/Picture11.png)

Based on the data, it seems that 2014 is when the company had the lowest averages within all the columns. On the other hand, the highest averages were mostly in 2020, although, the highest (low) average was in 2019. This may identify the continuous growth of the company, as the dataset showcases the history of stock prices from 2014-2020. Therefore, 2014 was the lowest and 2020 was the highest.  


### Question 3: Which month throughout the years had the highest average price? The lowest? 

The Highest averages:

![Data](/graph/Picture12.png)

There was no consistent month that had the highest average price, although November and December did have the highest average twice. December had the highest average in 2014 and 2020. November had the highest average in 2015 and 2018. This may be due to the specialty holiday drinks available. 

The Lowest averages:

![Data](/graph/Picture13.png)

Throughout the years, there was no consistent month that had the lowest average price. Although January had the lowest average twice in 2015 and 2019. May be due to the removal of the specialty drinks, and people are not spending money on coffee since this is after major holidays (where a lot of money is spent). 

![Data](/graph/Picture14.png)

![Data](/graph/Picture15.png)

## Discussion: 

Based on the analysis of Starbucks stock prices, it was concluded that the company is continuously growing. Although, there have been outside influences (which is inevitable) that may have affected this upwards trend. For example, the company peaked in 2020 but quickly started deescalating due to the declining economy from COVID-19. The lowest stock prices occurred in 2014, which may be the result of not gaining as much popularity, not enough investors, or possible controversy. When comparing the yearly averages, there was a relatively positive trend within the stock prices. Although, stocks are never linear. The price drops that occurred may have been due to economic struggle. The monthly analysis of the average stock prices showed a possible high in price due to seasonal menus, and a low due to possible need of saving money after a holiday season. Future research could include identifying patterns within the societal events within Starbucks and other coffee companies to identify if the trends are general or specific to Starbucks. 

## References: 

https://pandas.pydata.org/docs/reference/api/pandas.Series.reset_index.html

https://www.geeksforgeeks.org/pandas-series-dt-year/

https://matplotlib.org/stable/tutorials/pyplot.html

https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.sort_values.html

https://pandas.pydata.org/docs/reference/api/pandas.to_datetime.html

