# python-api-challenge
Module 6 challenge
# Libraries used in this analysis:
•	matplotlib.pyplot - for data visualization (plotting graphs)
•	pandas- for data manipulation and analysis (handling datasets)
•	numpy - for numerical operations (e.g., arrays, mathematical functions)
•	requests - for making HTTP requests to retrieve data from APIs
•	time - for handling time-related operations (e.g., delays, timestamps)
•	scipy import stats - for statistical functions (e.g., correlation, regression)
•	citypy - for working with city-related data (e.g., city coordinates, airport codes)
First, I generated random pairs of latitude and longitude coordinates. Using the citypy library, I then mapped each random pair of coordinates to the nearest city. 
After identifying the nearest cities for each set of coordinates, I used the OpenWeatherMap API to retrieve weather data for these cities. The weather conditions I focused on included:
•	Temperature 
•	Humidity 
•	Cloudiness 
•	Wind Speed 
This data was fetched using HTTP requests through the requests library. Each request was sent to the OpenWeatherMap API for the corresponding city, and the returned data was parsed in JSON format.
The weather data collected from the API was combined with the previously identified city and geographic coordinates (latitude and longitude). This was done by merging the weather information into a pandas DataFrame, ensuring that each row represented a unique city with associated weather conditions and coordinates.

I used matplotlib.pyplot to visualize the data and performed linear regression analysis using scipy.stats to explore how each weather condition correlated with latitude.
I applied linear regression to each weather index as the dependent variable, with latitude as the independent variable. The regression model helped quantify the relationship between latitude and each weather condition.
