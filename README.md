# 06-pythonAPIHW
Python API homework

## Part I - WeatherPy

I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator, utilizing a [simple Python library](https://pypi.python.org/pypi/citipy) and the [OpenWeatherMap API](https://openweathermap.org/api).

The first requirement is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

The second requirement is to run linear regression on each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

A CSV of all retrieved data and a PNG image for each scatter plot is in the WeatherPy/output_data folder.

#### Trends Observed in Part I



## Part II - VacationPy

Now let's parse the weather data to plan potential future vacations. The Google Places API is used for this part of the assignment.

To complete this part of the assignment, a heat map was created displaying the humidity for all cities from Part I.

The list of all cities is narrowed down to find my ideal weather condition. For example:

  * A max temperature between 75-85 degrees
  * Wind speed less than 10 mph
  * Zero cloudiness

  * Any rows that don't meet all three conditions was dropped.

* Using the Google Places API, the first hotel for each city located within 5000 meters of the coordinates was located.

* The hotels were plotted on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

* A screenshot of the final heatmap is included in the VacationPy folder.

#### Trends Observed in Part II