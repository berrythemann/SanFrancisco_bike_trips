# San Francisco Bay Area Bike-Sharing Data Exploration
## by Abdulmaleek Oladipo


## Dataset

This data includes information about individual rides made in a bike-sharing system
covering the greater San Francisco Bay area. It consists of 183412 row of trips and
16 features such as duration_sec, start_time, user_type, etc. The dataset can be 
downloaded using this [link](https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv)

## Summary of Findings

Before exploring, I carried out preliminary wrangling to extract days of the
week and hours of the day (which are features that would be required throughout
the analysis) from start_time.

In the exploration, I found out that Thursday is the day of the week with most
trips while 8am and 5pm are the time of the day bikes are mostly used.
I also discovered that duration has a long-tailed distribution, with a lot
of trips on the short duration end, and few on the long duration end. When
plotted on a log-scale, the trip duration distribution looks unimodal, with
the peak between 400secs and 700secs. Interestingly, there's a smooth ramp up
before the peak and a smooth ramp down after the peak.
Most of the bike users are subscribers, with just few customers. The bikes were
mostly used for trips by males.
While also exploring, I also noticed that user type doesn't have effect on bike
trips across each weekday.

Outside of the main variables of interest, I verified that the bike with the 
bike_id _4794_ was used for most trips.


## Key Insights for Presentation

For the presentation, I focused on the influence of user type on plot of trip
duration against weekday. I made use of faceted boxplot to make sure the 
difference between plot is clear.