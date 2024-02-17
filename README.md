# kai-python-api-challenge
## Part 1: WeatherPy
- In this deliverable, you'll create a Python script to visualise the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python library Links to an external site., the OpenWeatherMap API Links to an external site., and your problem-solving skills to create a representative model of weather across cities.
For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.
To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.
- Requirement
. Latitude vs. Temperature
. Latitude vs. Humidity
. Latitude vs. Cloudiness
. Latitude vs. Wind Speed

## Part 2 : VacationPy
- In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.
The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.
Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualisations.
To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:
Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.
https://static.bc-edx.com/data/dla-1-2/m6/lms/img/humidity_map.png

## Reference
- ChatGpt 
Convert 'Humidity' column to a list
size = city_data_df['Humidity'].tolist()

 Create a map plot with points representing cities and humidity as the size of the points
map_plot = city_data_df.hvplot.points(
    'Lng', 'Lat', size=size, geo=True, tiles='OSM', frame_height=600, frame_width=800
)
