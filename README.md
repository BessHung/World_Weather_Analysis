# World_Weather_Analysis

## Project Overview
Use OpenWeatherMap API and Google places API to retrieve the best cities for a vacation based on clients' weather preferences, and then find the nearest hotel for the cities and create a travel itinerary map.

## Process & Results
- Retrieve Weather Data 
1. Use the `NumPy` module to generate more than 2,000 random latitudes and longitudes.
2. Use the `citipy` module to list the nearest city to the latitudes and longitudes.
3. Use the **OpenWeatherMap API** to request the current weather data from each unique city in your list.
4. Collect the required data and save as [WeatherPy_Database.csv](https://github.com/BessHung/World_Weather_Analysis/blob/519fae46f65aef83997dda3cfe806bac73622ae2/Weather_Database/WeatherPy_Database.csv).
- Create a Customer Travel Destinations Map
1. Determine the weather preferences and filter from WeatherPy_Database.
2. Use **Google nearbysearch** to find the nearest Hotel of each city and save as [WeatherPy_vacation.csv](https://github.com/BessHung/World_Weather_Analysis/blob/519fae46f65aef83997dda3cfe806bac73622ae2/Vacation_Search/WeatherPy_vacation.csv).
3. Create a marker layer map with a pop-up marker for each city.
###### WeatherPy Vacation Map
![](https://github.com/BessHung/World_Weather_Analysis/blob/519fae46f65aef83997dda3cfe806bac73622ae2/Vacation_Search/WeatherPy_vacation_map.png)

- Create a Travel Itinerary Map.
1. Pick 4 cities from WeatherPy_vacation and create DataFrames for each city.
2. Use **gmaps direction layer** to create a direction layer map between the 4 cities.
3. Combine the four city DataFrames and create a marker layer map with a pop-up marker.

###### WeatherPy Travel Map
![](https://github.com/BessHung/World_Weather_Analysis/blob/519fae46f65aef83997dda3cfe806bac73622ae2/Vacation_Itinerary/WeatherPy_travel_map.png)

###### WeatherPy Travel Map Markers
![](https://github.com/BessHung/World_Weather_Analysis/blob/519fae46f65aef83997dda3cfe806bac73622ae2/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
