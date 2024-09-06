## UNIT-3

`Andrew Thomas`
`Overview of Project for Unit 3`

###        UNIT #3 : Applied Data Science with Python

Block 14: NumPy

Overview:

    As a data analyst at Weather Insights, a leading weather analytics company, you have been assigned the crucial task of analyzing and extracting insights from a dataset containing daily weather records. Your goal is to process the weather data using NumPy and derive meaningful conclusions that will help meteorologists and decision-makers understand patterns, fluctuations, and critical weather events. 
    
Scenario:

    Weather Insights has collected historical weather data for a specific location over the past week. The dataset, stored as a NumPy array, includes information about the date, temperature, humidity, and precipitation for each day. The management has tasked you with performing a comprehensive analysis to provide key insights. 
    
Dataset:

    The weather data is represented as a NumPy array with the following structure: 
    
    #Data in array format [date, temperature, humidity, precipitation] 
    
    weather_data = np.array([ 
    
        ["2023-07-01", 30, 60, 0.1], 
    
        ["2023-07-02", 31, 62, 0.2], 
    
        ["2023-07-03", 29, 65, 0.0], 
    
        ["2023-07-04", 33, 68, 0.5], 
    
        ["2023-07-05", 34, 70, 0.3], 
    
        ["2023-07-06", 32, 63, 0.1], 
    
        ["2023-07-07", 30, 61, 0.0] 
    
     ]) 
Directions:
    Perform the following analyses using NumPy and present your findings to the senior meteorologists at Weather Insights: 
    
    Calculate the average temperature for the entire dataset to provide an overall understanding of the weather conditions.Identify the hottest day during the week. Compute the temperature fluctuations over time to analyze the variability in daily temperatures. This        fluctuation is calculated by providing the difference in temperature between the current day and the previous day. Note that you will begin tracking temperature fluctuations starting from the second day (since we have nothing to compare for day 1).
    Identify days with high precipitation (precipitation above 0.2 inches) to highlight weather events with significant rainfall. 
    Calculate the average humidity for days with high precipitation to understand humidity levels during rainy periods. 
    Calculate the total precipitation for the entire dataset to quantify the overall rainfall experienced during the week. 
    Identify the coldest day during the week. 
    Filter data for summer days (temperature above 30 degrees Celsius) to analyze specific hot weather patterns. 
    Calculate the average temperature for summer days to provide insights into the temperature during the summer period. 
    Count the number of days with no precipitation to understand the frequency of dry days. 
    Prepare a comprehensive report with your analysis, insights, and visualizations to assist meteorologists in making informed decisions and understanding the weather trends in the specified location.


###    Block 15: Linear Algebra


Objective

    A linear regression model is being used to represent the relationship between the features (House area, Bedrooms, Bathrooms, and Garage size) and the target variable (Price in $) with the linear equation given below.


    Where a, b, c, and d are the coefficients of the linear equation.
    
    In a linear regression model, the coefficients can be calculated using the formula, image.png
    
    X = Matrix with independent variables (House area, Bedrooms, Bathrooms, and Garage size)
    
     y = Target variable (Price in $)

Your task is to build the house price prediction model using linear algebra principles in Python.

Directions

    1. Split the input dataset into two matrices: X contains all the features of the house, and y contains the target variable (Price).
    
    2. Create a function linear_regression() to calculate the coefficients of the linear equation using the formula: image.png
    
    Use NumPy functions to perform the matrix operations shown in the formula.
    The function should return the “coefficients” value as an output.
    3. Create the function estimate_house_price(coefficients, new_features) that predicts the price of the house.
    
    Calculate the estimate price with the dot product of the coefficients and the new features.
    Create a new_features matrix with the following values:
    House area = 1800 sq ft
    
    Bedrooms = 3
    
    Bathrooms = 2
    
    Garage size = 400 sq ft
    
    Call the function estimate_house_price() to predict the price of the new house.
    
    HINT: In order to split X from the y, use this code 
    X = data[:, :-1]
    
    y = data[:, -1]
    
    data = np.array([[1500,3,2,400,200000],
                     [1800,4,3,500,250000],
                     [1200,2,1,300,180000],
                     [2100,5,3,550,280000],
                     [1400,3,2,350,190000],
                     [1600,4,2,450,220000],
                     [1300,3,1,320,185000],
                     [2000,4,3,480,270000],
                     [1750,3,2,420,240000],
                     [2400,5,4,600,320000],
                     [1100,2,1,280,160000],
                     [1850,4,3,530,290000],
                     [2500,5,4,620,340000],
                     [1950,4,2,490,280000],
                     [1450,3,2,380,210000],
                     [1350,2,1,310,175000],
                     [2200,4,3,530,310000],
                     [2050,4,3,520,290000],
                     [1650,3,2,410,225000],
                     [2300,5,4,590,330000]])

###    Block 16: Working With Pandas


    Scenario:
    Suppose you are a data analyst working for a real estate company. Your manager has provided you with the "house_prices.csv" dataset and wants you to perform a preliminary analysis of the data to gain insights into the housing market. The company is interested in understanding the factors that influence house prices and wants to identify potential opportunities for growth in its business. 

Problem Statement:

    Write a Python code that utilizes the Pandas library to load, clean, and analyze the dataset. Generate visualizations using Pandas to better understand the relationships between house prices and various features. Present your findings and highlight any interesting trends or correlations that you discover during your analysis. 

Directions: 
    
    1. Import the necessary libraries and load the dataset into a Pandas DataFrame. 
    
    2. Perform basic data exploration and data cleaning if necessary. 
    
                 - display the first few rows
    
                 - display the shape of the dataframe
    
                 - display the size of the dataframe (aka the amount of cells or data points (row_count*column_count))
    
                 - display the number of NONE values in the dataset
    
            
    
    3. Answer a few key questions: 
    
    Calculate the average house price using .mean(). 
    Find the most common number of bedrooms and bathrooms. 
    Identify any correlation between the house price and other numeric features (e.g., sqft_living, waterfront, and view) using .corr() functions. 
    Calculate the average price of waterfront and non-waterfront houses. 
    Determine the average price of houses with different numbers of floors. 
    Analyze the average price based on the house condition. 
    4. Visualize the data using only Pandas plotting capabilities to create: 
    
    A histogram showing the distribution of house prices using .plot() 
    Scatter plots to visualize the relationships between price and other numeric features using .plot() 
    A bar graph to count the occurrences of each city 


###    Block 17: Statistics Fundamentals


Problem Statement: 

    As a data analyst for a retail company, your task is to conduct a comprehensive statistical analysis of the sales data using Python. 

Scenario: 

    You are a data analyst working for a retail company, tasked with analyzing sales data to gain comprehensive insights into the performance of different products. The dataset provided contains information about the sales of various products over a certain time period. Your goal is to perform a thorough statistical analysis using Python to answer specific questions about the sales data and present meaningful conclusions. 

Dataset: 

    Product A: [235, 189, 340, 270, 305, 210, 320, 265, 315, 280, 250, 200] 
    
    Product B: [320, 190, 340, 270, 310, 260, 315, 290, 320, 275, 230, 320] 
    
    Product C: [270, 290, 280, 240, 260, 210, 200, 340, 295, 280, 260, 310] 

Tasks to perform: 
    
    How does the total sales vary across different time periods within the dataset? 
    What is the daily average sales for each week/month during the observed time period? 
    Are there any seasonal trends or patterns in the sales data? 
    Can you identify any specific products that experienced significant sales fluctuations? 
    Which product categories contributed the most to the total sales? 
    Are there any correlations between sales of different products? 
    How does the coefficient of variation differ for various product categories? 
    Can you determine any outliers in the sales data, and how might they affect the analysis? 
    Is there any indication of improvement or decline in sales performance over time? 
    How can you utilize the sales data to inform marketing and inventory strategies? 
    Interpret the result. 
    Directions for the Workshop: 
    
    Calculate the total sales during the time period covered by the dataset. 
    Find the average daily sales during this time period. 
    Identify the best-selling product (highest sales) and its corresponding sales value. 
    Determine the worst-selling product (lowest sales) and its corresponding sales value. 
    Calculate the range of sales to understand the variability in the data. 
    Compute the standard deviation of sales to assess the spread of sales values. 
    Identify if the sales data is positively or negatively skewed. 
    Calculate the coefficient of variation for the sales data to compare the relative variability among products. 
    Determine the 25th percentile of sales, representing the sales value below which 25% of the products fall. 
    Compute the interquartile range (IQR) of sales to understand the middle spread of the data. 
    Finally, interpret the result. 


###    Block 18: Advanced Statistics


Scenario: 

    The city council of San Francisco is planning to increase the number of public parks in the city. They have been gathering data on the number of parks in different neighborhoods, along with data on the population density and average income of each neighborhood. The city council wants to understand whether the number of parks in each neighborhood is distributed randomly, or if it depends on the population density or average income of the neighborhood. 

Dataset:

    The dataset is provided with information about each neighborhood in San Francisco. The dataset includes the following fields: 
    
    - neighborhood: The name of the neighborhood 
    
    - num_parks: The number of public parks in the neighborhood 
    
    - pop_density: The population density of the neighborhood (people per square mile) 
    
    - avg_income: The average income of residents in the neighborhood 

 

Objective and Directions:

    Your task is to analyze this dataset and answer the following questions: 
    
    Is the distribution of parks across neighborhoods independent of population density? Use a chi-square test of independence to answer this question. Report the p-value, chi-square statistic, and degrees of freedom.
        - Null Hypothesis (H0): The distribution of parks across neighborhoods is independent of the population density. 
    
        - Alternate Hypothesis (H1): The distribution of parks across neighborhoods is not independent of the population density. 
    
    Is the distribution of parks across neighborhoods independent of the average income? Use a chi-square test of independence to answer this question. Report the p-value, chi-square statistic, and degrees of freedom.
        - Null Hypothesis (H0): The distribution of parks across neighborhoods is independent of the average income. 
    
        - Alternate Hypothesis (H1): The distribution of parks across neighborhoods is not independent of the average income. 
    
    For both the above questions, interpret the p-value and chi-squared statistic in the context of the problem.
    Calculate the correlation between the number of parks and the population density of each neighborhood. Interpret the correlation coefficient.
    Calculate the correlation between the number of parks and the average income of each neighborhood. Interpret the correlation coefficient.
    Based on your findings, provide recommendations to the city council about their plan to increase the number of public parks.
    Hints for Today's Workshop 18
    Use pd.qcut(<column>, q=4) to turn a numeric value into a categorical valueUse pd.crosstab to put your table together (frequency distribution for 2 categorical variables)Use chi2_contingency from scipy.stats to carry out the Chi-Square TestUse pearsonr from scipy.stats to carry out any correlation calculations
     
    
    Starter Code
    
    # Transform Data to Quartile Data (Numerical -> Categorical)
    df['pop_density_quartiles'] = pd.qcut(df['pop_density'], q=4)
    df['avg_income_quartiles'] = pd.qcut(df['avg_income'], q=4)
    df['num_parks_quartiles'] = pd.qcut(df['num_parks'], q=4, duplicates='drop')
    
    # Create Frequency Table based on the two variables you are interested in
    # Example
    contingency_table_pop = pd.crosstab(df['num_parks_quartiles'], df['pop_density_quartiles'])


###    Block 19: Data Analysis

Text Processing for a Document
Scenario: 

    You are working for a company that deals with many text documents. The company is interested in processing these documents to extract specific information, clean the text, and standardize the format for consistency. To accomplish this, you have been given a Python script that uses the re (regular expressions) module to perform various text processing tasks on a sample text document. 


Problem statement:
    You have to process the given sample text document, perform specific tasks using regular expressions, and write the modified text into a new file. 

Tasks to be performed:

    Search for the pattern ‘is' in the string and display the index of the matched object: ‘This is a sample string.’
    Find all occurrences of the word ‘sentence' in the string: ‘This is a sentence. This is also a sentence. Is this a sentence too?’.
    Extract all words from the list of email addresses given below. Also, extract the domain names from these email addresses.
    martin@gmail.com 
    
    thomas@stanford.edu 
    
    rose_11@fashion.now.inc 
    
    Extract all the phone numbers from the given string:
    ‘Emma changed her phone number from 0821-1234567 to 0800-1234567. Adam is still using 1234-1234567 as his number.’
    Replace variations of ‘Amrica' with 'America' in the ‘sample.txt’ file.
    Remove all instances where the characters ‘~' and ‘^' are followed by numbers from the ‘sample.txt’ file.
    Find all consecutive uppercase words in the ‘sample.txt’ file.
    Use a list comprehension to convert all uppercase words to lowercase from the ‘sample.txt’ file and store the result in the ‘lower_words' list.




Real Estate Data Analysis
Scenario: 

    You are working for a real estate agency that deals with data on house prices. The agency has collected data on house prices from various cities and wants to perform data analysis and queries on this dataset. To facilitate efficient data management and analysis, you have been provided with Python code that utilizes the SQLite and Pandas libraries.


Problem statement:

    Perform data analysis and querying on the HousePrices dataset using SQLite and Pandas. 

Dataset: 

    HousePrices.csvLinks to an external site.

Tasks to be performed:
    
    Import the pandas and SQLite3 libraries.
    Display the first few rows of the DataFrame to get an overview of the data.
    Create a connection to the database using SQLite3.
    Define the SQL query to retrieve all the data from the 'test' table where the 'city' column is equal to 'Seattle.
    Display the contents of the 'data' DataFrame to present the filtered house prices data for the city 'Seattle'.



###    Block 20: Data Wrangling


Overview: 

    This workshop is a comprehensive introduction to data analysis using the Pandas library in Python. The workshop will use the Titanic dataset, a rich dataset providing details about the passengers on the Titanic.
    
    Working with real-world data is often messy and unstructured. As a data scientist, you will frequently need to load data, clean it, handle missing values, preprocess it, merge it with other datasets, and visualize it to extract meaningful insights. You will gain hands-on experience with these tasks in this workshop, using the Titanic dataset as an example. 

Problem Statement: 

    You are a data scientist at a historical society dedicated to studying maritime disasters. The society has recently acquired a dataset about the Titanic passengers, and they want you to analyze this data to gain insights into the tragedy. The data includes various details about the passengers and their survival status. You need to perform data wrangling operations on the dataset provided, including data indexing, manipulation, handling null values, feature scaling, etc.

Directions: 

    Load the Dataset: Use read_csv() to load the Titanic dataset from a CSV file into a DataFrame. The DataFrame should now hold the entire dataset. 
    Explore the Dataset: Use methods such as head(), tail(), describe(), and dtypes to examine the data you are working with. 
    Index Manipulation: Use df.iloc[] and df.loc[] to access specific rows in the DataFrame. Set a new index for the DataFrame with df.set_index() and reset it with df.reset_index(). 
    Data Filtering: Save filtered data to a new CSV file using df.to_csv(). 
    Memory Optimization: Check the DataFrame's memory usage with df.memory_usage(). Optimize the memory usage by converting certain columns to a more memory-efficient data type using df.astype(). 
    Handle Missing Data: Use df.isnull().sum() to count null values in the DataFrame. Drop rows with null values using df.dropna(). Fill missing values in the DataFrame using df.fillna(). 
    Data Preprocessing: Normalize data using the Min-Max scaling technique. 
    Groupby Operations: Use the df.groupby() function to group data by a particular column and perform aggregate functions on these groups. 
    Data Visualization: You can use df.plot() to plot other types of charts, such as bar charts.  


###    Block 21: Data Visualization

Scenario:

    You are a manager at ABC Retail Company. The company has stores across different regions, and they have tasked you with building a dashboard to track key metrics across all their stores. The company has provided you with a dataset of transactions for the past year. Your task is to analyze and visualize the data using Python libraries.  

Problem Statement:

    Calculate the following metrics and create appropriate visualizations in Jupyter Notebook: 

    Distribution of the total revenue across different stores 
    Monthly trends in revenue 
    Top five products by sales volume  
    Comparison of quantity sold per category  
    A pivot table showing total revenue by store and by month  
    Which store has the highest average unit price for its products?  
    What is the revenue distribution for each category of products?  
    Create a scatter plot to show the relation between Quantity and Revenue for different categories.  
    
 Directions: 
    
    Initialization: 
    - Import the required libraries. 
    
    - Load the dataset into `df`. 
    
    - Calculate `Revenue` by multiplying `Quantity` and `Unit_Price`. 
    
    - Format the `Date` column to `datetime`. 
    
     Total Revenue by Store: 
    - Using `seaborn`, visualize a bar chart with stores on the x-axis and revenue on the y-axis, titled "Total Revenue per Store". 
    
     Monthly Revenue Analysis: 
    - Extract the month from `Date` and save the value in a `Month` variable. 
    
    - Calculate the monthly revenue and illustrate the trend using a Seaborn line chart. 
    
     Top Products Analysis: 
    - Calculate the total quantity sold for each product. 
    
    - Highlight the top five products with a bar chart. 
    
     Category-wise Quantity Analysis: 
    - Compute the total quantity for each category. 
    
    - Represent the results with a Plotly graph. 
    
     Revenue Pivot Table: 
    - Produce a pivot table showcasing revenue sums with stores as rows and months as columns. 
    
     Analysis of Store Unit Prices: 
    - Show the average unit price for products at each store using a Seaborn bar chart. 
    
     Category Revenue Distribution: 
    - Depict revenue distributions per category through a Seaborn box plot. 
    
     Quantity-Revenue Relationship: 
    - Demonstrate the correlation between `Quantity` and `Revenue` across categories using a Plotly graph. 

