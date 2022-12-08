# World_Weather_Analysis
## Travel itinerary project for routes

Code ref: Pandas, Python 3.7.6, Jupyter notebook, Geoapify API, Json

### Overview of Project

The purpose of this analysis was to identify possible cities within temperatrue range 65 - 90 degrees F to create a travel itinerary and display the route on a map. Utimatley, 4 cities would be chosen in a single country and a detailed route would be created on a map between the cities. Mexico was chosen and the four city include ["Tomatlan", "Pochutla", "Jungapeo", & "Acapulco"]. The nearest hotel was chosen as a waypoint within each city as a final destination coordinate.

## Dev 1: Retrieve weather data 
file reference: Weather_Database.ipynd, Weather.Database.csv
### Results: 
* Weather data was retrieved using the Geoapify weather API and placeing the data into a dataframe
<img width="944" alt="Weather_vacation_map" src="https://user-images.githubusercontent.com/115188500/206460765-370d6b90-90e1-4625-8676-c6baf23149f1.png">

## Dev 2: Create a Customer Travel Destination Map
file reference: Vacation_Search.ipynd, Vacation_Database.csv, Weather_Vacation_map.png
### Results:
* Customer requests 4 cities within a set max and min temperature range within the same country. A new dataframe was created to log all cities within this temperature range and create a map displaying all the cities. The hover function was used to display weather data when the user hovers over each city.
![Vacation_Itinerary_Cities](https://user-images.githubusercontent.com/115188500/206461490-169e1431-6053-4b8c-8d87-50e21d259f2e.png)


## Dev 3: Create a Travel Itinerary Map
### Results
* Customer requests to identify four cities to map a looping route between each city. Data was retrieved using the Vacation_Search Dataframe and the Geoapify Route API. Collected data using Json response and fetched each leg of th route to loop through. Coordinates where then put into a data frame and a map and path map were combined to show the route line.
![Vacation_itinerary_route_map](https://user-images.githubusercontent.com/115188500/206461533-08826d26-0085-42f4-8666-4e9aede86cd2.png)

### Additional
I was not able to confirm why the city points were no longer viewable with the route. I suspect it has something to do with the hv.plot function.
