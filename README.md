# Ford GoBike System Data Analysis
## by Jimmy Ogeto


## Dataset

- This dataset was provided by the Ford GoBike System covering the greater San Francisco Bay area between. The dataset is composed of records of all the bike rides that occured between 2019-02-01 and 2019-02-28. There are 183412 rows and 16 columns.
- There was a small number of rows with null values which I dropped. To make analysis easier, I created some columns from the availble data namely: hour, day, week, TOD, age, age_goup. 
- Most of the columns provided are self-explanatory except for a few. Here they are:
  - start_time, start_station_id, start_station_name, start_station_latitude, start_station_longitude.
  - end_time, end_station_id, end_station_name, end_station_longitude, end_station_latitude.
  - duration_sec, duration_minutes, bike_id, age, hour, day, week, member_birth_year, member_gender, 
  - user_type - (subscriber, customer)-Whether a bike rider is a subscriber of the service or a customer.
  - bike_share_for_all_trip- (yes, no)- whether a rider is part of the bikeshare program for low income residents or not.
  - TOD - (early_morning, morning, afternoon, night)- part of the day based on what time the bike ride took place.
  - age_group - (young, middle_age, old) - age group of the rider based on their age.   


## Summary of Findings

- The duration_minutes column has a largely long tailed distribution with a majoroty of the bike rides lasting between 1 and 40 minutes. In a logscale distribution,it can be seen that the distribution is slightly bimodal with a the first peak between 3-5 minutes and the other between 10 and 15 minutes.
- The distribution of the hours column is roughly bimodal with 2 peaks. The fist peak is at 8am and the other at 5pm. These 2 peaks indicate the times when most bike rides start. As compared to other parts of the day, it is in the afternoon(12pm-6pm) that a bulk of the bike rides take place. These 2 peaks could represent when most of the riders use the bikes to get to work and get back from work in the evening.
- The largest number of riders are young(114024), followed by middle_age riders(57398) and lastly seniors(3530). The age distribution is skewed to the right with a majority of the bike riders aged between 18 and 40 years
- The highest number of bike rides during the week happen on thursday.The weekends have the lowest number of bike rides for the whole week. This implies
- 74.5% of bike riders are male followed by 23.32% female bike riders.
- 90.53% of people who ride the bikes are subscribers of the service as opposed to 9.47% who are customers only.
- 90.1% of all bike riders have not enrolled for the bike-share for All program for low-income residents.
- The duration of bike rides during the peak hour of 7-9am and 4-6pm are less than 12 minutes on average. Which could indicate the most people riding a bike to work, do not work at places that are far away from bike stations.
- The average duration of rides vary very slighlty by age-roup, with young riders(18-35) having a low average while seniors(> 60 years) have a higher average.
- It is young people(18-35) that compose the largest group of bike riders throught the week.
- The number of bike riders who are subscribers is consistently higher than that of customers throughout the week.
- When it comes to subscribers it is male bike riders that are high in number followed by female bike riders and those who did not indicate their gender.
- The duration of bike rides during the peak hour of 7-9am and 4-6pm are less than 12 minutes on average. Which could indicate the most people riding a bike to work, do not work at places that are far away and are the same people who ride back in the evening. This could also mean that the duration of the bike rides is correlated to the time in which the bike ride is taking place.
- It is seen that day of the week has no corelation with user_type since, for all days of the week, the highest number of bike riders were subscribers.
- Average duration of bike rides throoughout the week is highest on the weekends for both subscribers and customers.

## Key Insights for Presentation

- Male bike riders are high in number followed by female bike riders and those who did not indicate their gender.
- The duration_minutes column has a largely long tailed distribution with a majoroty of the bike rides lasting between 1 and 40 minutes. In a logscale distribution,it can be seen that the distribution is slightly bimodal with a the first peak between 3-5 minutes and the other between 10 and 15 minutes.
- The average duration of rides vary very slighlty by age-roup, with young riders(18-35) having a low average while seniors(> 60 years) have a higher average.
- Subscribers on average, ride bikes longer thoughout the week and on the weekends, the customers and subscribers both have week high averages in duration of their bike rides.
- The distribution of the hours column is roughly bimodal with 2 peaks. The fist peak is at 8am and the other at 5pm. These 2 peaks indicate the times when most bike rides start. As compared to other parts of the day, it is in the afternoon(12pm- 6pm) that a bulk of the bike rides take place. These 2 peaks could represent when most of the riders use the bikes to get to work and get back from work in the evening.
- It is young people(18-35) that compose the largest group of bike riders throught the week.
- The number of bike riders who are subscribers is consistently higher than that of customers throughout the week.
