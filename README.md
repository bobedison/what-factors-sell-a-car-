# what factors sell a car?
 practicum project
# What Factors Sell a Car?

# Introduction

In this project an analysis of vehicle advertising data will be carried out. This project analysis will determine the factors that affect the price of a vehicle.

## Purpose

This project will test several hypotheses related to vehicle prices, namely:
1. The higher the age of the vehicle, the cheaper the price of the vehicle
2. The higher the odometer value, the cheaper the vehicle price
3. The higher the quality of the condition of the vehicle, the more expensive it is
4. Automatic transmission has a higher price because it is more comfortable
5. In general, black and silver cars have a higher after-sales price

## Stages 

In this project the dataset will be taken from /datasets/vehicles_us.csv, which is a collection of vehicle advertisement data that must be explored.

First, a review of this data will be carried out, then handling missing data, outliers to improve data quality and finally an analysis is carried out to answer the hypothesis that has been raised.

## This project will consist of 3 stages, namely:
1. Overview
2. Pre-processing
3. Hypothesis Test

Final conclusion
the analysis aims to examine datasets over the past few years and determine the factors that influence the price of a vehicle.
The following is a resume that has been done:
handle lost data:
1. there are 5 missing data columns model_year, cylinders, odometer, paint_color, and is_4wd
2. The model year column is the year of the vehicle which is difficult to find, so the missing data is deleted
3. column cylinders, odometer, filled with the median of the model and type of similar vehicles
4. column is_4wd is an index to determine the type of 4 wheel drive car, so missing data is replaced with a value of 0
5. paint_color column, missing data is filled with NA (not available) because the data is not very important and if deleted it will discard other data
handle data outliers:
1. odometer column = 0, while not a new car, filled with the median of similar models and types
2. Column price = 1, filled with the median of similar models and types
change data type:
1. change the data type of the column model_year, cylinder, odometer to integer
2. change the data type of the date_posted column to datetime
improve data quality:
1. Add a new column that contains the value of the time and date when the ad was shown
2. Added a new column containing the age of the vehicle when the ad was shown
3. Added a new column containing the average vehicle mileage per year
4. Added a new column containing the index of the car's condition
learn the core parameters
1. Study the core parameters, namely price, vehicle age, mileage, cylinder and condition
2. perform an analysis with a boxplot and clean out the outliers
analysis results
1. In general, ads run for 33-39 days
2. The 2 vehicles with the highest average prices are buses and trucks
3. The 2 vehicles with the most advertisements are sedans and SUVs
4. Automatic type transmission vehicles are more expensive than manual and other vehicles
5. Overall there is no significant color preference for price, yellow and orange are the color preferences with the highest vehicle prices
6. The older the vehicle, the cheaper the price, and vice versa
7. The lower the odometer value, the higher the price and vice versa
8. Cars in excellent conditions, like new and good have the highest prices with cars in excellent conditions having the highest number, while cars in fair and salvage conditions are the cheapest