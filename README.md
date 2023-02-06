## Python API Asssignment

# Summary

# WeatherPy

The Python code randomly selects a group of 500+ cities across the world. Then, the code collects data from the OpenWeatherMap API to create a representatitve model of weather across world cities. The API data is used to graph the following relationships:

Temperature (C) vs. Latitude

Humidity (%) vs. Latitude

Cloudiness (%) vs. Latitude

Wind Speed (mph) vs. Latitude

From the analysis, the following conclusions can be drawn:

    * For northern hemisphere, the relationship between Latitude and Max Temperature is negatively correlated;as latitude increases,Temperature decreases. This implies Temperature decreases as we move away from equator. The r value is also nearly 1. For southern hemipshere, the relation between Latitude and Max Temperature is very slight positively correlated; as latitude decreases(moving towards equator- as southern hemisphere has negative Latitude), temperature increases.
    *The correlation between Humidity and Latitude across Both hemispheres are really small. For northern hemisphere for some very high latitudes, there is a high humidity
    *There is nearly zero correlation between Cloudiness and Latitude across both hemispheres since the scatter plot has values distributed across the graph
    *No relationship can be defined between Latitude and Windspeed, Hence both of them have distributed values across the scatter plot

# VacationPy
For the second part of this project (VacationPy), I used the weather data gathered from part one to help plan for future vacations. Specifically, I used jupyter-gmaps and the Geopify Places API to create a Map that displays the humidity for every city from part one.

I then narrowed down the list of cities to find the ideal weather conditions, including:

    *A max temperature lower than 27C and greater than 21C
    *Wind speed less than 5 m/s.
    *Cloudiness less than 15%

I ended up dropping any rows that didn't contain all three conditions.

I then used the Geopify Places API to find the first hotel for each city located within 10000 meters of the coordinates. 

Finally, I plotted the hotels on a MAP with each hover showing the hotel name, city, and country.

Files

The analysis includes the following files:

A "WeatherPy.ipynb" Jupyter Notebook that contains the Python code for the analysis of partOne

A "VacationPy.ipynb" Jupyter Notebook that contains the Python code for the analysis of partTwo

A "api_keys.py" Python file that contains the OpenWeatherMap and Geopify Places API key used in the analysis. 

A "cities.csv" CSV file in the "Output" folder that contains the CSV version of the DataFrame created in the Jupyter Notebook

Four PNG files in the "Output" folder. Each of the four files is a graph created in the analysis
