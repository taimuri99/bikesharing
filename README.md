# Bikesharing
Module 14: NY Citibike with Tableau.
# Overview of the Analysis
Throughout the module, the main task was to analyse data from CitiBike for August of 2019. This was done as August was one of the more popular and active months for these services. The goal of the analysis was to see if a bike-sharing program in Des Moines was a solid business proposal and was sustainable. For this challenge we created 7 visualisations and added them to a Tableau story.
## Analysis of the module
The total number of rides were 2,344,224. The rides were divided amongst genders as so:

- Males : 1,530,272
- Females : 588,431
- Unknown : 225,521

The total rides were also divided by user type. Subscribers who had an annual subscription to the bike sharing service were comprised of 1,900,359 rides while customers who used it on a pay as you use basis comprised of 443,865. Additionally a plot was done to find the most popular riding times. 5 PM to 7 PM were the most busy and active hours. The least busy hours were between 1 AM and 5 AM therefore making it the prime time for repairs.

A plot was made to analyse age vs ride duration and the resulting trend showed that younger users used the bike services for longer durations. Finally bikes which had been ridden the longest distances and bikes which had been used the most were also plotted:

- BikeID 39570 travelled the largest distance/duration
- BikeID 38124 was the most actively used

The following is analysis of results for this challenge.

# Results
## Deliverable 1
For Deliverable 1, we used Jupyter Notebooks and panda dataframes to change the data type of the tripduration column from an integer to a datetime object. This was done so the visualisations for this challenge can be produced. 

<img width="999" alt="DFolddatatype" src="https://user-images.githubusercontent.com/87828174/143783314-d60a6d8c-a821-440c-9581-8e059b53c6fa.png">
<img width="1002" alt="DFnewdtype" src="https://user-images.githubusercontent.com/87828174/143783300-bf264b86-4c40-4f4f-a5c6-3c2a93a1b438.png">

The first image shows the original column and its values and the second image shows the values after being converted to datetime. The dataframe was converted to csv file and imported to Tableau to create the Viz. This code can be seen in NYC_Citibike_Challenge.ipynb

## Deliverable 2
The following 5 visualisations as tasked by the challenge to create are below. In addition 2 visualisations from the module are included as well.
### Checkout Times for Users

<img width="1026" alt="CheckoutTimesUsers" src="https://user-images.githubusercontent.com/87828174/143783517-fe35dc10-aec4-457e-bdce-a9f3f93c56a4.png">

This visualisation shows the number of bikes against trip duration or the length of time they are checked out for. The most popular trip duration was 5 minutes with 146,752 rides active for that duration. This plot is filtered on hours of trip duration and have the corresponding minutes of that hour on the x axis.

### Checkout Times by Gender

<img width="1029" alt="CheckoutTimesGenders" src="https://user-images.githubusercontent.com/87828174/143784510-53799c30-53a5-4b59-b4de-b640f7a2a93c.png">

This is a continuation of the previous plot in the same format. The checkout durations against number of rides is divided and filtered by gender and hours of trip duration. We see the most popular trip durations by gender:

- Male : 5 Minutes with 108,087 rides
- Female : 6 Minutes with 34,151 rides
- Unknown : 11 Minutes with 7,389 rides

An additonal note to remember is that males are more prevalent in using this service thats why the peak of the graph is much higher for them.

### Trips by Weekday for Each Hour

<img width="510" alt="TripsWeekDayHour" src="https://user-images.githubusercontent.com/87828174/143785366-78e43fec-7401-426c-828d-16977e212f28.png">

This plot shows a colour map showing activity of this service. The more reddish the colour, the more counts of rides in that time. Looking at this plot we see:

- 5 PM and 6 PM were the most active hours of the week. These hours were extremely popular on Monday, Tuesday and Thursday
- 8 AM was also very active for riders
- Saturday and Sunday were generally active throughout the day from 10 AM to 7 PM

From this plot one can see that there is a trend of rush hours being the most active time periods for riders both in the morning and evening.

### Trips by Gender (Weekday per Hour)

<img width="1439" alt="GenderWeekdayHours" src="https://user-images.githubusercontent.com/87828174/143790468-950e30cd-684a-45ce-aa32-1e0461e37541.png">

The previous analysis is filtered by gender. One can see the same trends being followed for all genders. The trend where the rush hours and weekends are the most active hours. One can also see that the darkest colours are with Males, then Females and lastly Unknown. This follows the same trend as found in the module where we saw the largest percentage of these bike users were Male and smallest percentage were Unknown.

### User Trips by Gender by Weekday

<img width="354" alt="TypeGenderWeekday" src="https://user-images.githubusercontent.com/87828174/143790899-f509b610-59ab-4dc9-9e21-f5783c1c2a7e.png">

The above viz showed activity per day filtered by genders and user types. Some of the findings are:
- There were more subscribers compared to customers for Males and Females while it was the opposite for Unknown
- Thursday for Males was the most active day for the bike service

### Top Starting Locations

<img width="1245" alt="TopStarts" src="https://user-images.githubusercontent.com/87828174/143791652-3b519eaa-9568-4509-8216-a61f6f53fee9.png">

The above plot is a heatmap for the most popular and active bike starting locations. We can see that the highest concentration of bike starting activity is in Southern Manhattan in Pershing Square North. The activity is centered in this location due to locations being closer together and bikes being more economic than cars as parking is expensive. Affordability and availability plays a key factor in the concentration of bike ride starting points here.

### Top Ending Locations

<img width="1242" alt="TopEnds" src="https://user-images.githubusercontent.com/87828174/143792726-9cb063fd-0383-408c-85be-fbbb156bb0e3.png">

This plot is similar to the previous one, the difference being that this is a plot of the most active ending locations. Similarly the most active location is Pershing Square North in southern Manhattan. 

# Summary
## Deliverable 3
Tasked to create a Tableau story for the challenge, the link is embedded here:
[Link to Tableau Story](https://public.tableau.com/app/profile/taimur.ahmad.khan/viz/Module_14_Challenge_16380498463870/KeyOutcomesoftheNYCCitibikeAnalysis)
Overall Analysis also embedded here:
[Module Analysis](https://public.tableau.com/app/profile/taimur.ahmad.khan/viz/Module14_16376370689200/NYCCitiBikeStory)
## High Level Summary
From this analysis we can understand that although New York and Des Moines are starkly different in size in population, there are some universal factors that can be implemented in both places:

- Bike service locations tend to be more active and popular in places where keeping a car is not financially economical
- Affordability and availability plays a key factor in the concentration of bike ride starting points
- Bikes are also used more actively in areas where the distances are smaller and and can be traversed by bike
- Subscribers and Males tend to make a larger share of users as compared to customers and other genders
- Early mornings (1 AM to 5 AM) are less busy and can be used to service or repair the bikes
- The most popular rides were those of a shorter duration from a range of 5 to 11 minutes for all genders
- Rush Hours and Weekends are more active time periods for rides
- 8 AM, 5 PM and 6 PM were the most active hours in the data throughout the week
- These trends followed similarly for all genders
- Younger users generally travelled larger distances/ had longer trip durations
- The most popular ride locations were in the heart of the city

## Two Additional Visualizations
1. Visualisation based on the most popular trip distances covered by plotting distance of ride versus ride counts. This can help us understand if larger or smaller distances were more popular and on average what distance travelled by bike was most common amongst the riders.
2. Visualisation based on which age used the bike service the most so we can see who our target audience will be.

