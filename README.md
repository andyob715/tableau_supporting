# Tableau Homework Submission

### Approach

I took the last 3 years of Citibike data csv files and used Pandas to clean a lot of the data.
The first thing I had to do was read in each csv file and merge them together.
The issue with that approach is that some of the columns changed during the scope of my dataset.

So I validated that each column headers and found which ones could be merged together.

I merged those together and then found the ZIP Code for each station with a free API that I found.

I grabbed the ZIP Codes for each station in the dataset by lat/long (this took a few iterations to get them all).

I could finally use that cleaned data to load into Tableau do some visual analysis.


### Insight #1 -- Geolocation Popularity

https://public.tableau.com/app/profile/andy.o.bryan/viz/Citibike_Analysis_Dashboard/StationLocationDashboard?publish=yes

This dashboard shows that popularity is centralized in one ZIP Code in the dataset, 07302.
Within that ZIP COde most of the Stations are seeing very similar popularity, which means that it's fairly distributed within the ZIP Code and not one Station pulling the average up.

The tree map shows the popularity of the start to end stations and as expected, most paths are coming from or going to the Grove St PATH area, which resides within 07302.

### Insight #2 - Month/Hour Popularity

https://public.tableau.com/app/profile/andy.o.bryan/viz/Citibike_Analysis_Dashboard_Popularity/PopularityDashboard?publish=yes

This dashboard shows that the popularity of the service (as expected) increases significantly in the Summer months.
Interestingly, the Average Distance and Average Duration of the trips does not change much throughout the month/hours.

As stated in the dashboard, this could mean that the weather is causing people to opt-in to the service, but not modifying their schedule/activities based on the weather.
If they were, I would have expected to see a higher duration and/or distance in those months/hours.

### Story

https://public.tableau.com/app/profile/andy.o.bryan/viz/Citibike_Analysis_Dashboard_Popularity/CitibikeStory?publish=yes

This story aggregates all of the data together. In all my years of interacting with people that use Tableau I have never seen anyone present a Story.

### Notes

In the Git repository I did not bring in each individual csv file or the exported files generated through the data cleansing process due to size/load constraints.
These can be provided upon request if required for grading the submission.

