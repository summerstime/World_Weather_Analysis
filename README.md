# Vacation Itinerary
Module 5 Project

## Overview

This project is to satisfy the requirements for the fifth module challenge in the Data Analysis Bootcamp. We are working with APIs. 
In this project we are asked to create a vacation itinerary based on the user's desired minimum and maximum temperatures.
A list of cities is generated and displayed on a map. The user is asked to enter the 4 cities they would like to visit.
A map of a directions is displayed through the cities, based on the order they were entered.
Also to with the list of cities the nearest hotel to the particular coordinates (latitude,longitude). 
A final map is displayed with only those 4 cities showing on the map.

## Results

### Weather Database
In Weather_Database, 764 pairs of coordinates, latitude and longitude, were randomly generated.
An API key was used when accessing the OpenWeatherMap.org to access the weather for those coordinates.
JSON data was reviewed to pull particular information from the data and a data frame was created. 
A total of 697 cities were found in the weather data and used for this project.
This dataframe was exported to a csv file named WeatherPy_Database.csv.
![Weather Dataframe](https://github.com/summerstime/World_Weather_Analysis/blob/main/Weather_Database/DF_Weather.png) 

### Vacation Search
In Vacation_Search, WeatherPy_Database.csv was read in so that it could be used.
Two input questions were asked of the user to know what minimum and maximum temperatures they would like for their vacation.
Those values were then used to reduce the size of the dataframe to only those cities that share the min/max values.
A total of 127 cities were found to fit the min/max temperatures. Hotels were also found for each of the cities.
Information was gathered using an API key and Google Map API information.
The information was exported to an output file called WeatherPy_Vacation.csv
![Vacation Search](https://github.com/summerstime/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png) 

### Vacation Itinerary
In Vacation_Itinerary, WeatherPy_Vacation.csv was imported. 
Four input questions were asked of the user to know the 4 cities that would be visited.
Those answers' latitude and longitude were gathered. The tuple function and to_numpy() was used to pair up each coordinate pair.
The Google Direction API was utilized to determine the route to visit the 4 cities chosen.
![City Map Information](https://github.com/summerstime/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png) 
Itinerary list 
![Itinerary List](https://github.com/summerstime/World_Weather_Analysis/blob/main/Vacation_Itinerary/Itinerary_list.png) 


## Summary
The final map show the 4 cities that user wants to visit. The information about the city is shown on the info card that pops up when the marker is chosen.
![Final Map](https://github.com/summerstime/World_Weather_Analysis/blob/main/Vacation_Itinerary/Final_map.png) 
  
