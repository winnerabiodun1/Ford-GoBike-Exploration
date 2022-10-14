# (Ford Go BIke Data Explaration)
## by (Winner Abiodun)


## Dataset

> Ford GoBike System Dataset was provided by Udacity and it includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. 

> Preliminary wrangling was done both visually but mostly programatically.
The Dataset contained 183412 observations with 16 features, 7 columns were type float and object respectively, the remaining was type int.

> Three main issues were resolved, The missing values, Incorrect data types and Irrelevant columns were dropped. After which the number of observations dropped to about 174952 rows and 13 columns with 6 columns of type category, 4 float columns and 2 columns for type int and object respectively.

> This analysis main area of interest and exploration was to see the How Trip Duration is affected by every column in the dataset, particularly Distance, Start Time, Age, USer type and Gender

## Summary of Findings

> The Trip Duration is Skewed and Most of the trip duration are between 100-1000seconds or 1-20mins. The dataset also had an unusual amount of outliers. The Duration was also converted from seconds to minutes which had values closely related to the logarithmic transformation of the duration in seconds, Hence the analysis was done using Duration in minutes. 
Compared to the distance, Most trips were between 0-10km and a duration of 80mins. Customers also spent higher time on trips than Subscribers, even though the number of customers are a mere fraction of the number of subscribers.
The same trend was seen in the gender, as the 'other' gender spent the highest time traveling. Uers between the ages 62-72 years old also spent the highest travel time. Longer time was spent on weekend Trips than weekdays.
Trips that also start beteen 2am-4am and trips that end between that time tend to be longer in duration than any other trip start and end time.
Those that dont use bikes for all round trips tend to spend higher time on trips than those that do not.


> The Start and end time columns were both splitted into Weekdays and Day Hours. They were very similar with only very slight differences. Hence most of the analysis was done focuing on the start time mostly. However, the data was only for the Month of February in the year 2019.
Most of the Trip Counts started and ended on Tuesdays, Wednesdays, Thursdays, and Fridays. 
Most Trips also started and ended by 5pm, 8am, 6pm, 9am and 4pm.

> The Busiest start stations was Market st at 10th st with over 3500 trips generated. The Busiest stop station was San Francisco Caltrain station 2 with over 4500 stops. The End stations Had more traffic generally than the start sations.

> Over 90% of Bike users are Subscribers, others are Customers.

> Over 70% of bikers are males, 23% Females and the rest ar of gender 'other'
This acconts for the male count spike across the comparism of the categorical variables

> 90% of bike users dont use BIkes for all round trips
No customer uses bike for all round trips not even 1.

> A new column 'distance' was extracted from the start and end station latitude and longitude. and most frequent trips are between 0.5-3km.
Customers cover longer distances than Subscribers. As well as the 'other' gender. Those that do not use bikes for all round trips cover more distance in transit than those that do.
Trips that start and end between 2am and 10am are longer travels.
Long Distance trips tend to start and end between Tuesdays and Fridays.
Age groups over 95years are have the longest trip distance coverage in the entire dataset


> The Age of the bike users as at 2019 was deduced from their birth year and then an age group was formed with users between the ages 29-39 years having the most counts with over 7000 appearances followed by users between the age 18-28years. 
The age group 18-28years are mostly active at late nights between 9pm-4am, while the group 29-39years are nore active from 5am-8pm



## Key Insights for Presentation

> For the presentation, The Influence of all the categorical columns on the Trip Duration, Trip Distance and The Trip start and end time was discussed.

> This includes Discussing each categorical variable as it relates to the variable of interest

> I started by introducing the Trip duration and distance, then the start and end week days and hours. The User type, gender, Bike usership for allround trips and Age groups were all discussed under the univarite analysis using piecharts and histograms.

> For the Bivariate Analysis, The Relatinship between the Trip duration and Distance was explored using a scatterplot, then the Trip Duration and start week days and hours, usertype, gender using pointplots.
Trip Distance was also explored for Start Hours and Weekdays with pointplots

> For the Multivariate Analysis, Trip Duration, Bike Usership for All Trips and Age Group, Trip Distance User Type and Start Hours, Trip Duration and Start Hours Across Gender were all explored using pointplots, Trip Duration, Age Groups and Weekdays, Trip Duration, Weekdays, Gender and User Type, Trip Distance, Weekdays, Gender and User Type were explored using Heatmaps