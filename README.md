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
 HOT SPOTS : Road Crashes 2020
  
<p align="center"> 
  <img width="563" alt="Screen Shot 2021-06-05 at 10 32 47 PM" src="https://user-images.githubusercontent.com/63677816/120911850-1233cc80-c650-11eb-9104-bd61d5501e60.png">

<p align="center"> 
  LOCATION : FATAL CRASHES
  
<p align="center"> 
  <img width="538" alt="Screen Shot 2021-06-05 at 10 49 55 PM" src="https://user-images.githubusercontent.com/63677816/120911929-b3bb1e00-c650-11eb-8d4f-1a1e118f7f3d.png">
  
  <p align="center"> 
  CRASHES AGGREGATED TO ROAD NETWORKS 
  
  <p align="center"> 
    <img width="505" alt="Screen Shot 2021-06-05 at 10 54 55 PM" src="https://user-images.githubusercontent.com/63677816/120911978-1ad8d280-c651-11eb-9d02-727e224c5643.png">

 <p align="center"> 
  SPEED CAMERA LOCATIONS: 
  
  <p align="center"> 
      <img width="549" alt="Screen Shot 2021-06-05 at 10 57 04 PM" src="https://user-images.githubusercontent.com/63677816/120912042-93d82a00-c651-11eb-99d0-9bc7acb66231.png">

<p align="center"> 
  STREET NETWORKS WITH MAXIMUM CRASHES : Results Queried From PostgreSQL
  
<p align="center"> 
  <img width="547" alt="Screen Shot 2021-06-05 at 11 05 04 PM" src="https://user-images.githubusercontent.com/63677816/120912152-7d7e9e00-c652-11eb-9708-906f19b28edc.png">

  
#### DISCUSSION :
  1. We can see that there is a jump in Road Crash fatalities for the year 2020 which are significantly higher compared to other years especially for the month July but we also see immediate kinks for the subsequent months. 
  2. The top 5 street networks that have the maximum crashes are the follwing street no. 1600, 7900, 800, 200, 100. 
  3. Although the speed cameras can reduce police enforcment and possible incidents of racial profiling, it has not been very well received with Chicago. Speed Cameras have worked really well in France and have brought about behavioural changes in motorists given how efficiently they have been placed across road intersections where there are threats to vulnerable road users such as pedestrians. One of the reasons that it was not taken so well in many of the cities in United States is because it was seen as revenue raising gimmick by the government. 
Speed Cameras if placed strategically and equitably have the possibility to reduce serious and fatal crashes (more on that later), while reducing the potential for racially-biased traffic enforcement by police officers.
 Currently the fine is $35 for travelling 6-10 MPH over the applicable speed limit within a Children’s Safety Zone.  The fine is $100 if the recorded speed of the vehicle is 11 or more MPH over the applicable speed limit. From an economic standpoint and something I learnt in the class : Health Impacts of Transportation reducing the dollar price of fines but increasing the number of tickets can actually bring significant behavior changes in motorists. 

#### LIMITATIONS:
I had very ambitious plans for this project but I ended up spending ample of time looking for relevant data sources and working with street networks and aggregations. I wasn't able to implement some of the models taught in class that I inteded to because of the data and format concerns. I was interested in showing statiscally significant clustering patterns in traffic crashes. 
  
#### CONCLUSION : 
Road accidents have been on the rise since the rapid motorization of cities and decreased reliance on public transit compared to individualized transport modes especially in American cities. There is a need to develop and implement policies that de-incentivizes or increases the costs of risk-taking behavior among road users through installation of speed cameras and other enforcement measures. There is merit in also understanding where these accidents take place frequently so strategic measures can be taken to reduce them.
We cannot simply advocate for modal shifts from individualized modes to active travel, public transit without understanding the exposure these modes impose on each other. In a transport environment where we have heavily invested in muti-lane roads to reduce congestion and enabled cars to drive at high speeds, we have to think about the risk they impose on vulnerable road users such as pedestrians and cyclists whose numbers increased during the pandemic. 
  
#### SCOPE FOR FUTURE WORK : I am interested in actually looking at the interactions in terms of crashes for these modes, for ex how many of these fatalities were caused by a collision between a car and a pedestrian or a cyclist. Having this data along with the spatial attribute can help us identify junctions that are the most dangerous. 
  

  
