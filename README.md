# World Weather Analysis
_An Analysis of Weather Data Using API calls_


## Overview of the Project

A good travel experience is always affected by the climate or weather condition of the destination. As most travellers decide on their trips, weather patterns become an important factor and information on this key element of travel sorted after the more.
This project was undertaken to improve a travel app by using input statements and API calls to help clients create a travel itinerary based on their weather preference.

The key goals for the project included:
- Produce travel destination based on customer's weather preference.
- Generate a list nearby hotels from travel cities.
- Create a travel itinerary 
- Produce a map to show travel plan


## Results

* **Weather Database**
Using the numpy module with the random function, 2,000 cordinates were generated to help produce city destinations.
The list of possible cities was generated from the cordinates after the citipy module was applied on the cordinates.
In order to get the weather condition of these cities required using API calls to OpenWeatherMap to obtain current weather. 
A DataFrame was then created to hold the infomation retrieved from the call.

_Below is an example of the  DataFrame that was generated_

![city_data](https://user-images.githubusercontent.com/100079292/162348096-156e6293-0a26-4aba-881b-7415256917a1.PNG)


* **Vacation_Search**
Prefered weather was collected from clients using input statements where clients could enter the maximum and minimum temperatures they desire.
These values were then used to generate cordinates to produce list of prefered cities from the weather database file.
Next an API call to google maps returned nearest hotels to possible city destinations.
Using info_box_template and list comprehension a marker layer map was produced to show cureent weather conditions for possible hotel locations around the world.

_Example of google maps with markers for current weather condition_

![Alt text](https://github.com/emmanuelbrim/World_Weather_Analysis/blob/main/Vacation_Search/Weather_vacation_map.PNG)


* **Vacation_Itinerary*
The creation of the vacation_itinearry involved the use of Google maps API to map out a sample itinerary from 4 cities that a client would prefer to visit based on the weather. The result showed a clean route of travel between four cities in South Africa. 


Example of google maps with markers for current weather condition_

![Alt text](https://github.com/emmanuelbrim/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

## Summary
Though the analysis done in this project answered the request of the Election Commission, it must be stated that with some modifications to the script used a more indepth information could be generated from this audit. 
The same Resources folder used here can hold data from other elections and with a change in the variables of the script to reflect that particular dataset, produce a whole new output upon request. On the other hand a decision statement could be introduced in the original script to generate votes per candidate in each county. This will tell how each candidate performed in each county. 
