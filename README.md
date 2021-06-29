![](https://github.com/npvandyke/World_Weather_Analysis/blob/main/banner.png)
# World Weather Analysis
Analyze & visualize current weather data for over 500 cities across the world. Generate destinations and itineraries using Google Maps Platform APIs. 

## Purpose: 
A use-case for this project includes user-interface enhancement for travel apps through the provision of filterable hotel destinations based on user-selected weather preferences. 

Other use-cases could be educational in nature, with interactive heat maps displaying a variety of weather parameters, and scatter plots and linear regression analyses showing the relationship between weather parameters and latitude. 

## Tools: 
- Software: 
  - Anaconda Navigator, Conda, Jupyter Notebook 
- Languages/Dependencies: 
  - Python, pandas, numpy, matplotlib, citipy, requests, datetime, gmaps 
- API Data Sources: 
  -    [OpenWeatherMap](https://openweathermap.org/current) 
  -    [Google Maps and Places](https://developers.google.com/maps/documentation/places/web-service/search) 
  -    [Google Maps Directions](https://developers.google.com/maps/documentation/directions/overview)

## Method: 

- Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. [Link to code.](https://github.com/npvandyke/World_Weather_Analysis/blob/main/Weather_Database/Weather_Database.ipynb) 
  - Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
  - Use the citipy module to list the nearest city to the latitudes and longitudes.
  - Use the OpenWeatherMap API to request the current weather data from each unique city in the list.
  - Parse the JSON data from the API request, collect the city weather data and add it to a DataFrame:

| City Data DataFrame | 
:-------------------------:|
![city_data_df](weather_data/city_data_df.png)  


- Create a Pandas DataFrame with hotel names for each city that meets the user's inputted weather criteria. [Link to code.](https://github.com/npvandyke/World_Weather_Analysis/blob/main/VacationPy.ipynb)
  -   Write two input statements that prompt the user to enter their minimum and maximum temperature criteria for their vacation.
  -   Filter the city_data_df DataFrame for the collected temperature criteria and create a new Pandas DataFrame.
  -   Use the Google Maps and Places API to request the nearest hotel for each city in the DataFrame. 
  -   Parse the JSON data from the API request, collect the hotel data and add it to the DataFrame: 
  
| Hotel Data DataFrame |
:-------------------------:
![hotels_df](weather_data/hotels_df.png)


- Create a heatmap with pop-up markers that can display weather and hotel information for specific cities based on the user's travel preferences. [Link to code.](https://github.com/npvandyke/World_Weather_Analysis/blob/main/VacationPy.ipynb)

- Create a itinerary map with four hotels that fit the user's selected criteria and directions between each destination. [Link to code.](https://github.com/npvandyke/World_Weather_Analysis/blob/main/Vacation_Itinerary/Vacation_Itinerary.ipynb)

![Vacation_Itinerary](Vacation_Itinerary/WeatherPy_travel_map_markers.png)

## Exploratory Analysis with Visualization

<b>Matplotlib-generated scatter plots comparing weather parameters at various latitudes:</b>

|                          |                           |
:-------------------------:|:-------------------------:
![Lat_vs_Max_Temp](weather_data/Fig1.png) | ![Lat vs Humidity](weather_data/Fig2.png)
![Lat vs Cloudiness](weather_data/Fig3.png) | ![Lat vs Wind Speed](weather_data/Fig4.png)



<b>Further exploration of the relationship between temperature and latitude using linear regression:


|  Northen Hemisphere | Southern Hemisphere |
:-------------------------:|:-------------------------:
![Lat_vs_Max_Temp](weather_data/temp_northern.png) | ![Lat vs Humidity](weather_data/temp_southern.png)

Questions? Comments? [Let's Connect!](https://www.linkedin.com/in/natalie-vandyke-npv/) ![](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)
