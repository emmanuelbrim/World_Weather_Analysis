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



* **Total Votes and Percentage of Votes per County**

One request from the Election Board was to generate the total number of votes cast in each county and the percentage of that to the overall votes cast in the election.
To honor this, two data structures; "county_list" and "county_votes" dictionary were created to hold data. 
A script to extract all county names was added under a For loop; "row in reader:" by assiging the second index to the variable "county_name".
Next an if statement was introduced to help obtain the values for the county list and county votes.
The final value for county_votes was based on increasing it by 1 after each loop.


_Example of code used to generate total votes per county_

![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/Total%20Votes%20per%20county.PNG)



The Percentage of votes per county was determined by dividing the total votes per county(ie the values in the county_votes dictionary) by the total votes cast in the election and multipling the results by 100.
The Votes_percentage variable was assigned with the results of this mathematical operation to provide the percentage of votes per county.
An f'string statement was then printed to terminal to show results.

_Example of code to generate percentage votes per county_

![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/votes%20per%20county.PNG)



_Example of F'string statement and terminal results of script_

![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/F%20string%20county%20votes%20and%20percentage.PNG)


![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/terminal%20view.PNG)




* **Largest Turnout County**

To find the county with the largest turnout required the introduction of two new variables; "winning_county count" and "winning_county".
Next a decision statement was created to determine the winning county and its vote count.
The results printed to terminal showed that Denever had the largest turnout with 306,855 votes.


_Example of decision statement and terminal results of largest turnout county_

![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/largest%20turnout.PNG)


![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/wining%20county.PNG)


* **Total Votes per Candidate and Percentage**

A similar outline like that used in generating Total votes per county was used to provide the total candidate votes. 
An initail candidate_votes dictionary and candidate_options list was created to hold data.
All candidate names were extracted from the third index after looping through all the rows in the CSV file.
Next, an if statement was introduced to generate total candidate votes by increasing the value of candidate_votes by 1 under the for loop "row in reader".
A second for loop was then created to loop through candidate_votes by candidate_name to get the unique votes per candidate which was assigned to the "votes" variable. Then the results of dividing votes by total votes multiplied by 100 was given as vote percentage.

_Example of code to generate percentage votes per candidate_

![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/percentage%20votes%20per%20candidate.PNG)


![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/terminal%20percentage%20vote%20per%20candidate.PNG)


* **Winning Candidate**

From the analysis of the data set it was revealed that Diana DeGette won the election with 272,892 votes being 73.8% of the total votes cast.
The winner was arrived at by the use of an if statement to generate winning_count and winning_percentage fromm the candidates_votes and vote_percentage respectively.

_Example of code to generate winning Candidate_

 
![Alt text](https://github.com/emmanuelbrim/Election_Analysis/blob/main/Resources/winning%20candidate.PNG)

## Election Audit Summary
Though the analysis done in this project answered the request of the Election Commission, it must be stated that with some modifications to the script used a more indepth information could be generated from this audit. 
The same Resources folder used here can hold data from other elections and with a change in the variables of the script to reflect that particular dataset, produce a whole new output upon request. On the other hand a decision statement could be introduced in the original script to generate votes per candidate in each county. This will tell how each candidate performed in each county. 
