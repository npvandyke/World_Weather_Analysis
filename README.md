# World Weather Analysis
Analyzing the relationship between latitude and a variety of weather parameters for over 500 cities around the world. 

## Purpose: 
PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.
## Method: 
Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. 
## Tools: 

## Collect the Data

- Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
- Use the citipy module to list the nearest city to the latitudes and longitudes.
- Use the OpenWeatherMap API to request the current weather data from each unique city in my list.
- Parse the JSON data from the API request.
- Collect the following data from the JSON file and add it to a DataFrame:
City, country, and date
Latitude and longitude
Maximum temperature
Humidity
Cloudiness
Wind speed

## Exploratory Analysis with Visualization

- Create scatter plots of the weather data for the following comparisons:
Latitude versus temperature
Latitude versus humidity
Latitude versus cloudiness
Latitude versus wind speed

|                          |                           |
:-------------------------:|:-------------------------:
![Lat_vs_Max_Temp](weather_data/Fig1.png) | ![Lat vs Humidity](weather_data/Fig2.png)
![Lat vs Cloudiness](weather_data/Fig3.png) | ![Lat vs Wind Speed](weather_data/Fig4.png)


- Determine the correlations for the following weather data:
Latitude and temperature
Latitude and humidity
Latitude and cloudiness
Latitude and wind speed
- Create a series of heatmaps using the Google Maps and Places API that showcases the following:
Latitude and temperature
Latitude and humidity
Latitude and cloudiness
Latitude and wind speed
Visualize Travel Data

## Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. 
