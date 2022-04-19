# python-api-challenge

## What's the Weather Like?

### Background

Using Python requests, APIs, and JSON, we are set off to answer "what's the weather like near the equator?". I know you maybe thinking that it's "hot" of course. But, can you prove it? 

We have delved into the financial, education, and healthcare world for real-world data scenarios. Now, it's time to use tools such as Python request, APIs, and JSON to answer questions definitively, sush as weather, poverty areas, food security, and much more. Our challenge is to answer "What's the weather like as you go near the equator?" We do this with two challenges: **WeatherPy and VacationPy**. See below to understand what we did to answer the latter question.

###  WeatherPy

The WeatherPy script will help to visualize the weather of 500+ cities of varying distance from the equator using simple Python library (https://pypi.python.org/pypi/citipy) and OpenWetherMap API (https://openweathermap.org/api). We will show the following:

### Scatterplots

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs Latitude

Within the script, you will find an explanation of what the code is analyzing. The second requirement is as follows:

### Linear Regression

> Each relationship is computed with the linear regression.
> Separate the plots into Northern (greater than 0 degrees latitude) and Southern Hemisphere (less than 0 degress latitude).

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

Each pair of plots will explain what the linear regression is modeling. The final notebook for **WeatherPy** will have at least 500 unique citites based on latitude and longitude. The latter will have performed a weather check on those cities using a series of successive API calls. A print log of each city with the city number and name will be saved to a csv file as well. 

### VacationPy

Vacation time! The **WeatherPy** must have been a lot! Let's jump into something more relaxing: **VactionPy**. We are taking our skills we used from the **WeatherPy** challenge to plan future vacations using Jupyter-gmaps and Google Places API. The following will be created:

* Heat Map: Displays the humidity for ever city from **WeatherPy**
* DataFrame: Displays ideal weather conditions such as max temperature lower than 80 degress but higher than 70, wind speedless than 10 mph, zero cloudiness, and delete any rows that do not meet those conditions.
* Find first hotel for each city located within 5,000 meters of coordinates
* Plot hotels on top of heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**.
