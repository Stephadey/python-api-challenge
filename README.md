
# # python-api-challenge

## Introduction

This project consists of two main parts: `WeatherPy` and `VacationPy`. The `WeatherPy` notebook focuses on gathering weather data from cities across the globe to analyse various weather patterns in relation to their latitude. The `VacationPy` notebook uses the weather data to identify ideal vacation spots based on specific weather criteria and visualises them using maps.

## Dependencies

-   Python 3
-   Jupyter Notebook
-   pandas
-   matplotlib
-   NumPy
-   requests
-   time (part of Python's standard library)
-   datetime (part of Python's standard library)
-   scipy
-   os (part of Python's standard library)
-   json (part of Python's standard library)
-   pprint (part of Python's standard library)
-   folium
-   [OpenWeatherMap API](https://openweathermap.org/api)
-  [Geoapify API](https://myprojects.geoapify.com)

## Installation

To run these notebooks, you need to install the required Python packages. You can install them using pip. Ensure you have Python and pip installed on your system, then run the following command in your terminal or command prompt:

`pip install pandas matplotlib numpy requests scipy folium`

Note: API keys for OpenWeatherMap and Geoapify are required to fetch the data.

## Usage

1.  Open the `WeatherPy.ipynb` notebook in Jupyter and run the cells to perform the weather data analysis.
2.  Open the `VacationPy.ipynb` notebook in Jupyter. Ensure you have set up your  API key correctly, and run the cells to identify potential vacation destinations.

## Features

-   `WeatherPy`: Analyses weather data from over 500 cities worldwide, exploring the relationship between latitude and weather phenomena such as temperature, humidity, cloudiness, and wind speed.

![enter image description here](https://github.com/Stephadey/Images/blob/main/all%20plots.png?raw=true)

-   `VacationPy`: Utilises weather criteria (e.g., temperature range, wind speed, cloudiness) to identify and map ideal vacation spots, integrating hotel information near these locations.

![enter image description here](https://github.com/Stephadey/Images/blob/main/maps.png?raw=true)

## Linear regression analysis

**Cloudiness vs. Latitude:**

-   The Southern Hemisphere showed a moderate positive correlation between cloudiness and latitude, with a higher tendency for cloudiness to increase closer to the equator. In contrast, the Northern Hemisphere displayed a weaker positive correlation. This suggests that while there is a general trend of increasing cloudiness with decreasing latitude, the relationship is not strong and likely influenced by other factors.

**Max Temperature vs. Latitude:**

-   A strong negative correlation was observed in the Northern Hemisphere, indicating that maximum temperatures decrease as one moves away from the equator. The Southern Hemisphere exhibited a moderate positive correlation, with temperatures increasing closer to the equator. Latitude appears to be a more significant predictor of temperature in the Northern Hemisphere compared to the Southern Hemisphere.

**Humidity vs. Latitude:**

-   A moderate positive correlation was noted in the Northern Hemisphere for humidity and latitude, whereas the Southern Hemisphere showed a weak positive correlation. This suggests that latitude has some influence on humidity levels, but other environmental factors likely have a stronger impact, especially in the Southern Hemisphere.

**Wind Speed vs. Latitude:**

-   There was virtually no correlation between wind speed and latitude in the Northern Hemisphere, and only a slight inverse relationship in the Southern Hemisphere. This indicates that latitude is not a significant factor in predicting wind speed in either hemisphere, with other geographical and meteorological conditions exerting more influence.

**Conclusion:** Across the different climate variables, latitude showed varying degrees of correlation with cloudiness, temperature, and humidity, but consistently little to no correlation with wind speed. The strongest relationship was between latitude and maximum temperature in the Northern Hemisphere, while other relationships ranged from moderate to weak. These variations suggest that while latitude can be a factor in climate patterns, its influence is not uniform across different climate variables or hemispheres. Other factors such as ocean currents, atmospheric circulation, geographic terrain, and local weather systems are likely to play crucial roles. Hence, while latitude is a valuable component in understanding climate behaviour, it cannot be relied upon as the sole predictor due to the complexity of the climate system.

## References
-   [OpenWeatherMap API](https://openweathermap.org/api)
-  [Geoapify API](https://myprojects.geoapify.com)
- https://realpython.com/python-folium-web-maps-from-data/ used to create map visuals in VacationPy
- https://pypi.org/project/citipy/
