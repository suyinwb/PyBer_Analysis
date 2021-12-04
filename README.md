# PyBer Analysis

## Background
V. Isualize has given me and Omar a brand-new assignment. Using my Python skills and knowledge of Pandas, I have to create a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, create a multiple-line graph that shows the total weekly fares for each city type. Finally, I will submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer.

## Overview of Project
Deliverables for the analysis of the school district:
* create a summary DataFrame of the ride-sharing data by city type
* create a multiple-line graph that shows the total weekly fares for each city type
* summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer

### Purpose

Results:
* Summary DataFrame of the ride-sharing data by city type
* multiple-line graph that shows the total weekly fares for each city type
* Summary of  how the data differs by city type and how those differences can be used by decision-makers at PyBer

## Analysis And Challenges

## Methodology: Analytics Paradigm

#### 1. Decomposing the Ask
We have 2 datasets that shows:
* city_data.csv -  city name, driver counts in the city, type of city_data
* ride_data.csv -  city name, date of each ride, fare of each ride, ride id
After we merged these 2 datasets, we will be able to generate summaries for the rides by city type and visualise total weekly fares for each city type.

#### 2. Identify the Datasource
* city_data.csv
* ride_data.csv

#### 3. Define Strategy & Metrics
**Resource:** Python 3.6, Anaconda, Jupyter Notebook

1. Merge the 2 datasets
1. Find total rides, total drivers, total fares, average fare per ride and average fare per driver.
1. Find the sum of fares by city type and dates
1. Group the fares weekly for date between '2019-01-01' and '2019-04-28'
1. Create a multiple line chart for the weekly fares data above.

 #### 4. Data Retrieval Plan
Read CSV with pandas
```
city_data_to_load = "resources/city_data.csv"
ride_data_to_load = "resources/ride_data.csv"
city_data_df = pd.read_csv(city_data_to_load)
ride_data_df = pd.read_csv(ride_data_to_load)

```

#### 5. Assemble & Clean the Data
* Merge the 2 datasets
* Group by city type and dates


#### 6. Analyse for Trends
Analyse trends for 2019 Q1 between the different city types.

#### 7. Acknowledging Limitations
* Self limitations with matplotlib, therefore reference Stackover Flow multiple times.

#### 8. Making the Call:
The "Proper" Conclusion is indicated below on [Summary](#summary)

## Analysis

Below is the summary of rides, drivers and fares by city types from the 2 datasets received.

>Summary of Rides, Drivers & Fares by City Types

![Pyber summary df](analysis/Pyber_summary_df.png)

From this summary, we can see that rural cities have the lowest number of rides and drivers but highest average fare per ride at $34.62 and highest average fare per driver at $55.49.
Even though urban cities have the highest total rides and total drivers, the average fare per ride and average fare per driver is the lowest among all city types. When we examine closer at the data, urban city type has more drivers, total of 2405, than rides, total of 1625. This means there is 48% more drivers to rides hailed.
The other 2 city types have higher rides compare to drivers respectively.

>Summary of Rides, Drivers & Fares by City Types

![Pyber summary](analysis/PyBer_fare_summary.png)


## Summary
Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.

From the analysis above, the most significant differences are due to Thomas High Schools' academic dishonesty are:

1. Thomas High School overall scores fell from _**90.94% to 65.07%**_. This means _**25.9%**_ discrepancy.
1. Thomas High School math scores fell from _**93.27%% to 66.91%**_. This means _**26.36%**_ discrepancy.
1. Thomas High School reading scores fell from _**97.3% to 69.66%**_. This means _**27.64%**_ discrepancy.


## Appendix
