# Bikesharing
Module 14 Tableau: NY Citibike with Tableau
# Overview of the Analysis
Throughout the module, the main task was to analyse data from CitiBike for August of 2019. This was done as August was one of the more popular and active months for these services. The goal of the analysis was to see if a bike-sharing program in Des Moines was a solid business proposal and was sustainable. For this challenge we created 7 visualisations and added them to a Tableau story.
## Analysis of the module
The total number of rides were 2,344,224. The rides were divided amongst genders as so:

- Males : 1,530,272
- Females : 588,431
- Unknown : 225,521

The total rides were also divided by user type. Subscribers who had an annual subscription to the bike sharing service were comprised of 1,900,359 rides while customers who used it on a pay as you use basis comprised of 443,865. Additionally a plot was done to find the most popular riding times. 5 PM to 7 PM were the most busy and active hours. The least busy hours were between 1 AM and 5 AM therefore making it the prime time for repairs.

A plot was made to analyse age vs ride durationa and the resulting trend showed that younger users used the bike services for longer durations. Finally bikes which had been ridden the longest distances and bikes which had been used the most were also plotted:

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

- 5 PM and 6 PM were the most active hours of the week. These hours were extremely popular on Monday, Tuesday and Thursday. 
- 8 AM was also very active for riders
- Saturday and Sunday were generally active throughout the day from 10 AM to 7 PM

### Trips by Gender (Weekday per Hour)
### User Trips by Gender by Weekday
### Top Starting Locations
### Top Ending Locations
# Summary
## Deliverable 3
Tasked to create a Tableau story for the challenge, the link is embedded here:
[Link to Tableau Story](https://public.tableau.com/app/profile/taimur.ahmad.khan/viz/Module_14_Challenge_16380498463870/KeyOutcomesoftheNYCCitibikeAnalysis)
## High Level Summary
## Two Additional Visualizations

