### Final Project GIS-III

#### RESEARCH QUESTION 

Severe traffic crashes cause serious death and injuries which negatively impacts public health, economic development and equity. The COVID 19 pandemic has transformed mobility in cities and the its impact on Chicago has been interesting in terms of total number of fatalities for the year 2020. Through this project, I have used various visualizing techniques to show the change in traffic crashes and fatalities over the past few years particularly concentrating on the year 2020. The project also tries to identify road networks that can be considered as 'hot spots' for road traffic accidents and targeted interventions can be made to brimg behavioral changes in road users. 

#### GOALS
1. To visualize the change in Road traffic crashes and fatalities in the past 4 years and identify the underlying causes for the same. 
2. Aggregate road traffic crashes in the year 2020 to street networks in Chicago : this would give us an idea about highways/streets where majority of the crashes take place
3. Provide recommendations for locating speed cameras along routes where over-speeding is a problem
4. Use PostgreSQL to query routes and their locations with maximum crashes for the year 2020. 

#### BACKGROUND AND MOTIVATION:
The year of 2020 turned out to be quite interesting in terms of Road safety statitics for the city of Chicago. I come from a city called Begaluru in India that is considered to have the worst traffic congestion in the country and the pandemic managed to reduce the total number of deaths that happen at a larger scale because of the reduction in traffic fatalities. To compare the results with Chicago, street networks saw a decrease in congestion which can impact speeds of the moving traffic. According to Chicago Department of Transportation (CDOT), Chicago saw a 35% increase in traffic deaths compared to 2019 which can be attributed to the documented increase in speeding due to low congestion. 

#### DATA SOURCES : 
1. **National Highway Traffic Saftey Administration (NHTSA)** :The query tool allows users to construct customized queries using data not only from NHTSA’s Fatality Analysis Reporting System (FARS) but also from the Crash Report Sampling System. 

<img width="911" alt="Screen Shot 2021-06-05 at 7 26 38 PM" src="https://user-images.githubusercontent.com/63677816/120910770-3f2fb180-c647-11eb-810c-c495aa090237.png">

2. **Chicago Data Portal** : Locations for speed cameras 
                             Traffic Crashes ( years 2016-2021) 
                         

#### METHODS USED 
1. Trends in Traffic Fatalities : Time series plot of fatal injuries 
2. Density of accidents in Chicago : 
   Fatalities : Creating hot spots using Open Street Maps (OSM) for Chicago | Plotting crash locations 
   Number of Crashes for the year  : Aggregating crashes to nearest road networks (I could've done better with this by showing multiple bin sizes but was      unable  to) 
 3. Buffer Analysis : Coverage for speed cameras (Literature review to get an idea about their efficacy) 
 4. Identifying the top 5 road networks and their location that have the maximum number of crashes : Querying Crashes_2020 data using PostgresSQL
 
   
#### RESULTS: 
<p align="center"> 
TIME SERIES PLOT : Road Crash Fatalities for the years 2018- 2021
  
<p align="center">
<img width="769" alt="Screen Shot 2021-06-05 at 10 20 37 PM" src="https://user-images.githubusercontent.com/63677816/120911351-80769000-c64c-11eb-95ec-338d32d27f9d.png">

<p align="center"> 
 

Dights
Limitations, Future Work, Conclusion
