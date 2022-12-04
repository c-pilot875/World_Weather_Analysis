# World_Weather_Analysis
## Travel itinerary project for routes

Code ref: Pandas, Python 3.7.6, Jupyter notebook, Geoapify API, Json

### Overview of Project

The purpose of this analysis was to identify possible cities within a certain temperature range to create a travel itinerary and display the routes on a map. Utimatley 4 cities would be chosen in a single country and a detailed route would be created on a map between the cities.

## Dev 1: Retrieve weather data 
file reference: Weather_Database.ipynd, Weather.Database.csv
### Results: 
* Weather data was retrieved using the Geoapify weather API and placeing the data into a dataframe

## Dev 2: Create a Customer Travel Destination Map
file reference: Vacation_Search.ipynd, Vacation_Database.csv, Weather_Vacation_map.png
### Results:
* Customer requests for identidying cities within a set max and min temperature range. A new dataframe was created to log all cities within this temperature range and create a map displaying all the cities. The hover function was used to display weather data when the user hovers over each city.

## Dev 3: Create a Travel Itinerary Map
### Results
* Customer requests to identidy 4 cities to map a looping route between each city. Data was retrieved using the Vacation_Search Dataframe and the Geoapify Route API. I was able to collect the data in Json format but was unable to figure out how to fetch the specific legs of the trip and display on a map. 
