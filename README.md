# Citibike Project: From NYC to Des Moines

Using Tableau to visualize bike sharing data

## Overview of analysis

This project is intended to help Kate pitch a potential business idea to an angel investor. Based on the success of the Citibike operation in New York City, this proposed business would instead take place in Des Moines, Iowa. A datafile of bike trip information from August 2019 was obtained and is the source of the analyses. 

### Deliverables

- An .ipynb file that changes the trip duration column's datatype from integer to datetime.
- A Tableau story consisting of at least seven visualizations of the NYC Citibike datafile.
- This README explaining the analysis

### Resources

- Files: 201908-citibike-tripdata.csv
- Technology: Tableau, Python, Jupyter Notebook

## Results

### Deliverable One

In order to create visualizations that can accurately display trip durations, the trip duration column of the data file was converted from integer datatype to datetime datatype. This was done in a Jupyter Notebook .ipynb file. The csv file was loaded as a Pandas dataframe, the column converted, and the dataframe exported as a new csv file.

### Deliverable Two

In order to sway the potential angel investor, a number of visualizations were created to illistrate the success of New York City's bike share program. In the order they are presented in the Tableau story: 

1. User Type

![User Type](https://github.com/josephrodini/bikesharing/blob/main/Images/CustomerUser.PNG?raw=true)

This pie chart shows the distribution of subscribers to non-subscribing customers for the NYC Citibike program. Over 80% of the users are subscribers.

2. User Gender

![Gender Type](https://github.com/josephrodini/bikesharing/blob/main/Images/GenderUser.PNG?raw=true)

This pie chart shows the distribution of genders of the bike users. The majority of users are male.

3. and 4. Checkout Times

All Genders Combined
![Checkout Combined](https://github.com/josephrodini/bikesharing/blob/main/Images/CheckoutCombined.PNG?raw=true)

This line chart shows the distribution of bike trips by duration, with all genders combined. The vast majority of trips are less than an hour, with the mode being less than ten minutes.

Separated by Gender
![Checkout Gendered](https://github.com/josephrodini/bikesharing/blob/main/Images/CheckoutGendered.PNG?raw=true)

This line chart shows the distribution of bike trips by duration, separated by gender. The pattern of short trips holds for all genders, though the distribution is slightly less skewed (more normal) for women and even more so for unknown gender.

5. and 6. Heatmap of Bike Trips by Weekday

All genders combined
![Heatmap Combined](https://github.com/josephrodini/bikesharing/blob/main/Images/WeekdayTripsCombined.PNG?raw=true)

This heatmap shows the density of trips taken for each hour of each weekday. The peak ridership times are during the morning and evening commute hours, approximately 6-10a.m. and 4-8p.m., respectively, on Monday through Friday. The weekends show a different pattern of steady, but lower, ridership all afternoon.


Separated by Gender
![Heatmap Gendered](https://github.com/josephrodini/bikesharing/blob/main/Images/WeekdayTripsGendered.PNG?raw=true)

This heatmap shows the density of trips taken for each hour of each weekday, separated by gender. In general, females show the same pattern as males, while there is no clear pattern of higher usage for those not providing a gender.

7. August Hours

![August Hours](https://github.com/josephrodini/bikesharing/blob/main/Images/AugustTrips.PNG?raw=true)

This bar chart shows the bike trips per hour during August 2019, one of the busiest months of the year. In addition to corroborating the finding of the heatmaps (that the morning and afternoon commutes represent the heaviest usage), we can also more clearly see the times of the day with the lowest usage. Ridership is lowest from 2-4a.m., which means this time is the best for bike repairs and maintenance.

8. User Trips by Gender by Weekday

![User trips by gender by weekday](https://github.com/josephrodini/bikesharing/blob/main/Images/CustomerGenderTrips.PNG?raw=true)

Finally, this heatmap shows a breakdown of ridership along the crossing of gender and user type. The greatest density of trips are being taken by male subscribers. Female subscribers outnumber female customers, while unspecified gender customers outnumber unspecified gender subscribers.

## Summary

Overall the visualizations paint a promising picture for the city of Des Moines. The Citibike program in New York City seems to be thriving, and with some modifications to the program, a version could easily prove successful in the Iowa city. There is high subscribership among both genders, and heavy usage during multiple parts of the day.

### Additional Visualizations

In order to gain more understanding of the data, it is suggested that visualizations be made showing:

- Trip duration by time of day: It would provide insight to see if the trips during the highest density rental times are longer or shorter than those during other times of the day. This way we could see if extra support would be needed during these peak hours.
- Trip duration by starting and ending location: It would also be interesting to see what stations have the longest and shortest trips taken between them. This could impact bike placement.

### Limitations

New York City is much more sizeable than Des Moines. It would still be prudent to conduct research on a city of similar population and density as Des Moines before proceeding.