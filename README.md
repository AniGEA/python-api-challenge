# Module 6 Challenge


Note: The provided API keys are solely for demonstration purposes within the existing Python codes. If users wish to access additional features or conduct further investigations, they are required to obtain their own API key. 


This activity is broken down into two deliverables, WeatherPy and VacationPy.
# * Part 1: WeatherPy

This analysis explored the relationship between latitude and key weather parameters across different hemispheres. Various insights into regional climate variations were sought by examining how latitude influences temperature, humidity, cloudiness, and wind speed. This exploration contributes to a better understanding of the complex interplay between geography and weather dynamics, facilitating informed decision-making in various sectors.

Northern Hemisphere:
Temperature vs. Latitude:

The moderately strong negative relationship (R-squared = 0.7382) suggests that latitude significantly influences temperature in the Northern Hemisphere.
The equation of the regression line indicates that as latitude increases (moves away from the equator towards the poles), temperature tends to decrease.
This relationship is expected due to the tilt of the Earth's axis, causing lower temperatures at higher latitudes.
Humidity vs. Latitude:

Although there's a positive relationship between humidity and latitude, the R-squared value (0.1733) suggests that latitude alone may not adequately predict humidity levels.
Other factors such as proximity to bodies of water, prevailing winds, and local geography may play significant roles in humidity variation.
Cloudiness vs. Latitude:

Cloudiness shows a weak positive relationship with latitude, indicating that cloud cover tends to increase slightly as we move towards higher latitudes.
However, the low R-squared value (0.0649) implies that latitude may not be the primary factor influencing cloudiness in the Northern Hemisphere.
Wind Speed vs. Latitude:

The negligible R-squared value (0.00032) suggests that latitude alone is not a significant predictor of wind speed in the Northern Hemisphere.
Wind patterns are influenced by various factors such as pressure systems, temperature differentials, and local geography, which may overshadow the effect of latitude.
Southern Hemisphere:
Temperature vs. Latitude:

A moderate positive relationship (R-squared = 0.5118) indicates that latitude influences temperature in the Southern Hemisphere.
As latitude increases (moves closer to the equator), temperature tends to rise, which aligns with expectations of warmer climates near the equator.
Humidity vs. Latitude:

The weak positive relationship between humidity and latitude (R-squared = 0.0362) suggests that latitude alone may not be a strong predictor of humidity levels in the Southern Hemisphere.
Other factors such as proximity to oceans, prevailing winds, and local geography may have more significant impacts on humidity.
Cloudiness vs. Latitude:

Similarly to the Northern Hemisphere, cloudiness in the Southern Hemisphere exhibits a weak positive relationship with latitude (R-squared = 0.0290).
While there's a slight increase in cloudiness towards higher latitudes, latitude alone may not be the primary determinant of cloud cover.
Wind Speed vs. Latitude:

In the Southern Hemisphere, latitude shows a weak negative relationship with wind speed (R-squared = 0.0467).
This suggests that, on average, wind speed tends to decrease slightly as latitude increases, but the effect size is relatively small compared to other factors influencing wind patterns.


# * VacationPy

This analysis explores weather data extracted from a list of cities across the globe. The data includes parameters such as temperature, humidity, wind speed, and cloudiness. Below is a summary of the steps and insights derived from the provided code:

A geographical plot is generated to visualize city humidity levels using latitude and longitude coordinates.
The size and color of the plot points correspond to humidity levels, providing an overview of humidity distribution across cities.

Hotel Search Based on Criteria:

Cities meeting specific weather criteria (temperature between 21°C and 27°C, wind speed less than 4.5 m/s, and cloudiness equal to 0) are selected.
Any rows with null values are dropped to ensure data integrity.

A new DataFrame, hotel_df, is created to store city information and the nearest hotel's name.
Hotel Search Using Geoapify API:

The Geoapify API is utilized to search for hotels near each selected city based on its latitude and longitude.
The search iterates through the hotel_df DataFrame, making API requests and storing hotel names.
If no hotel is found within the specified radius, "No hotel found" is assigned.

Visualizing Hotel Locations:

Another geographical plot is generated to display the selected cities along with their nearest hotels.
The plot points indicate city locations, and the hotel names are displayed upon hovering over the points.


# *Instructions

This activity is broken down into two deliverables, WeatherPy and VacationPy.
# Part 1: WeatherPy

In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python library Links to an external site., the OpenWeatherMap API Links to an external site., and your problem-solving skills to create a representative model of weather across cities.
For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.
To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.
Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude

To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:
Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed
Requirement 2: Compute Linear Regression for Each Relationship

To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.
Next, create a series of scatter plots. 

You should create the following plots:
Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude
After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.
# Part 2: VacationPy

In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.
The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.
Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.
To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:
Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.You should create the following plots:
Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude
After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.
Part 2: VacationPy

In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.
The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.
Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.
To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:
Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.
Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
A max temperature lower than 27 degrees but higher than 21
Wind speed less than 4.5 m/s
Zero cloudiness
