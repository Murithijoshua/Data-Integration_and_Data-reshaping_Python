# Data_Integration_and_Data-reshaping_Python
 Integrate several datasets into one single schema and find and fix possible problems in the data with Python.
 
## Introduction
 For this assessment, you are required to write Python (Python 2/3) code to integrate several datasets into one single schema and find and fix possible problems in the data.
 
## Data Integration
In this task, you are required to integrate these datasets into one with the following schema.

COLUMN
ID Address
Price Type
DESCRIPTION
A unique id for the property The property address
The property price The type of property
        
Suburb (15/100)
The property suburb. The suburb must only be calculated using Vic_suburb_boundary.zip.
Default value: “not available”
      
  Date Rooms Bathroom
Car LandSize Age Latitude Longitude
distance_to_train_station (5/100)
Date of sold
Number of bedrooms Number of bathrooms
The number of parking space of the property The area of the property
The age of the property at the time of selling The Latitude of the property
The Longitude of the property
The ​direct distance from the closest train station (identified above) to the property. ​Default value: -1
                            
train_station_id (15/100)
The closest train station to the property that has a direct trip to the Southern Cross Railway Station. A direct trip is a trip where there are no connections (transfers) in the trip from the origin to the destination. ​Default value: -1
travel_min_to_CBD (15/100)
The average travel time (minutes) from the closest train station (regional/metropolitan) that has a direct trip to the “Southern Cross Railway Station” on weekdays (i.e. Monday-Friday) ​departing ​between 7 to 9:30 am. For example, if there are 3 direct trips departing from the closest train station to the Southern Cross Railway Station on weekdays between 7-9:30 am and each takes 6, 7, and 8 minutes respectively, then the value of this column for the property should be (6+7+8)/3.). ​Default value: -1
over_priced? (4/100)
A boolean feature indicating whether or not the price of the property is higher than the median price of similar properties (with respect to bedrooms, bathrooms, parking_space, and property_type attributes) in the same suburb on the year of selling. ​Default value: -1
crime_A_average (3/100)
The average of type A crime ​in the local government area ​the property belongs to, in the three years prior to selling the property as the property. For example, if a property is sold in 2016, then you should calculate the average of the crime type A for 2013, 2014 and 2015. Default value: -1
 
 
