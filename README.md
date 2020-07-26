# Data_Integration_and_Data-reshaping_Python
 Integrate several datasets into one single schema and find and fix possible problems in the data with Python.
 
## Introduction
 For this assessment, you are required to write Python (Python 2/3) code to integrate several datasets into one single schema and find and fix possible problems in the data.
 
## Data Integration
In this task, you are required to integrate these datasets into one with the following schema.

Description of the final schema:
- ID: A unique id for the property 
- Address: The property address
- Suburb: The property suburb. The suburb must only be calculated using Vic_suburb_boundary.zip. Default value: “not available”
- Price: The property price 
- Type: The type of property
- Date: Date of sold
- Rooms: Number of bedrooms 
- Bathroom: Number of bathrooms
- Car: The number of parking space of the property 
- LandSize: The area of the property
- Age: The age of the property at the time of selling
- Latitude: The Latitude of the property 
- Longitude: The Longitude of the property
- Train_station_id: The closest train station to the property that has a direct trip to the Southern Cross Railway Station. A direct trip is a trip where there are no connections (transfers) in the trip from the origin to the destination. Default value: -1
- Distance_to_train_station : The direct distance from the closest train station (identified above) to the property. Default value: -1
- Travel_min_to_CBD: The average travel time (minutes) from the closest train station (regional/metropolitan) that has a direct trip to the “Southern Cross Railway Station” on weekdays (i.e. Monday-Friday) departing between 7 to 9:30 am. For example, if there are 3 direct trips departing from the closest train station to the Southern Cross Railway Station on weekdays between 7-9:30 am and each takes 6, 7, and 8 minutes respectively, then the value of this column for the property should be (6+7+8)/3.). Default value: -1
- Over_priced?: A boolean feature indicating whether or not the price of the property is higher than the median price of similar properties (with respect to bedrooms, bathrooms, parking_space, and property_type attributes) in the same suburb on the year of selling. Default value: -1
- Crime_A_average: The average of type A crime in the local government area the property belongs to, in the three years prior to selling the property as the property. For example, if a property is sold in 2016, then you should calculate the average of the crime type A for 2013, 2014 and 2015. Default value: -1
- Crime_B_average: The average of type B crime in the local government area the property belongs to, in the three years prior to selling the property as the property. For example, if a property is sold in 2016, then you should calculate the average of the crime type B for 2013, 2014 and 2015. Default value: -1
- Crime_C_average: The average of type C crime in the local government area the property belongs to, in the three years prior to selling the property as the property. For example, if a property is sold in 2016, then you should calculate the average of the crime type C for 2013, 2014 and 2015. Default value: -1
- Closest_primary_school: The name of the closest primary school to the property. Default value: “not available”
- Distance_to_closest_primary: The direct distance between the property and the closest primary school. Default value: -1
- Primary_school_ranking: The ranking of the closest primary school to the property as scraped from http://www.schoolcatchment.com.au/?p=12301If the school is not listed, the value of this field should be set to “not ranked”. Default value: -1
- Closest_secondary_school: The name of the closest secondary school to the property. Default value: “not available”
- Distance_to_closest secondary: The direct distance between the property and the closest secondary school. Default value: -1
- Secondary_school_ranking: The ranking of the closest secondary school to the property as scraped from https://sites.google.com/a/monash.edu/secondary-school-r anking If the school is not listed, the value of this field should be set to “not ranked”. Default value: -1

## Data reshaping
In this task, you need to study the effect of different normalization/transformation methods (i.e. standardization, min-max normalization, log, power, and root transformation) on Rooms, crime_C_average, travel_min_to_CBD, and property_age attributes. 
You need to observe and explain their effect assuming that we want to build a linear model on price using these attributes as predictors of the linear model and recommend which one(s) do you think would work better on this data. When building the linear model, the same normalization/transformation method can be applied to each of these attributes.

## Authors

Tangwei, Hung

## Contact
hung.tangwei@gmail.com
 
 






        



 
 
