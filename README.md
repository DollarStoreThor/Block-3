# UNIT-3

My repository for UNIT 3 of my fullstack AI and ML Course

UNIT #3 : Applied Data Science with Python

Block14: NumPy
Overview
As a data analyst at Weather Insights, a leading weather analytics company, you have been assigned the crucial task of analyzing and extracting insights from a dataset containing daily weather records. Your goal is to process the weather data using NumPy and derive meaningful conclusions that will help meteorologists and decision-makers understand patterns, fluctuations, and critical weather events. 

Scenario
Weather Insights has collected historical weather data for a specific location over the past week. The dataset, stored as a NumPy array, includes information about the date, temperature, humidity, and precipitation for each day. The management has tasked you with performing a comprehensive analysis to provide key insights. 

Dataset
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
Directions
Perform the following analyses using NumPy and present your findings to the senior meteorologists at Weather Insights: 

Calculate the average temperature for the entire dataset to provide an overall understanding of the weather conditions.Identify the hottest day during the week. Compute the temperature fluctuations over time to analyze the variability in daily temperatures. This fluctuation is calculated by providing the difference in temperature between the current day and the previous day. Note that you will begin tracking temperature fluctuations starting from the second day (since we have nothing to compare for day 1).
Identify days with high precipitation (precipitation above 0.2 inches) to highlight weather events with significant rainfall. 
Calculate the average humidity for days with high precipitation to understand humidity levels during rainy periods. 
Calculate the total precipitation for the entire dataset to quantify the overall rainfall experienced during the week. 
Identify the coldest day during the week. 
Filter data for summer days (temperature above 30 degrees Celsius) to analyze specific hot weather patterns. 
Calculate the average temperature for summer days to provide insights into the temperature during the summer period. 
Count the number of days with no precipitation to understand the frequency of dry days. 
Prepare a comprehensive report with your analysis, insights, and visualizations to assist meteorologists in making informed decisions and understanding the weather trends in the specified location.


Block 15: Linear Algebra


Objective

A linear regression model is being used to represent the relationship between the features (House area, Bedrooms, Bathrooms, and Garage size) and the target variable (Price in $) with the linear equation given below.

image.png

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

Block 16: Working With Pandas

Block 17: Statistics Fundamentals

Block 18: Advanced Statistics

Block 19: Data Analysis

Block 20: Data Wrangling

Block 21: Data Visualization
