# Cyclistic-Case-Study

## SCENARIO 

You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations.


## Preparing and Cleaning Data

The data is present in CSV files conssisting of 12 identical columns, which makes joining the 12 CSV files for the 12 years I will be working on very simple
I used R language to Read and Merge the CSV files that included the data from August 2021 to July 2022.

Following that I dropped any rows that have null values using the ommit() function.

After that to make sure there are no duplicate data I used  distinct() function to remove any possible duplicates.

## Transforming the Data

After checking the data types of each column, I discovered that the started_at and ended_at were of type string and not datetime, as such I converted I converted them to datetime using POSIXct() function.

Following that I used the mutate function to add a new column duration to easily calculate the avg trip duration more easily.

Finally I imported the data to a local postgresql database to use SQL to do the analysis.


## The Analysis

In this step I analyzed the 
