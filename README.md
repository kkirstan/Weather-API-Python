# Python API Homework - What's the Weather Like?

# Background

In this challenge I analyzed weather data, using the OpenWeatherMap API and the Google Places API to gather my data. 

# Part 1 - Weather Py

In this section, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a simple Python library and the OpenWeatherMap API to create a representative model of weather across world cities.

First I created a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

Then I ran linear regression on each relationship. This time, separating the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

Final notebook should:
Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it's being processed with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot.

# Part 2 - VacationPy

For this section, I used weather data collected from the previous step to plan future vacations. I also used jupyter-gmaps and the Google Places API for this part of the assignment.


Create a heat map that displays the humidity for every city from Part I.

Narrow down the DataFrame to find your ideal weather conditions. Mine were:


A max temperature lower than 85 degrees but higher than 75.


Wind speed less than 8 mph.


Zero cloudiness.


Drop any rows that don't contain all three conditions.

Use Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.


For Part I, I included a written description of three observable trends based on the data in the beginning of my main code, WeatherPy.ipynb.
For Part II, I included a screenshot of the heatmap I created in the VacationPy folder ("hotel_heatmap.png").
