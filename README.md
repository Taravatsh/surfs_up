# Surfs_up

## Overview of Project

In this project, we are willing to invest our savings in opening a Surf and Ice Cream shop in Oahu, Hawaii. After putting together a strong business plan we reach out to an investor for this matter. However, the investor wants to learn more about the weather consition in Oahu prior to making a commitment in building the shop as a result he requires us to perform some analytics on the weather by providing us with the dataset he has on the island.

### Purpose 

The purpose of this project to provide the investor with additional analysis about the temperature trends specifically for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is going to be sustainable year-round or not. As a result SQLAlchemy has been used as a query tool for SQLite where the data is stored in to perform the required queries for running the data in addition to Python, Pandas functions and methods.

## Results

In this section of the project Python, Pandas functions and methods as well as SQLAlchemy was used for determining the summary statistics of the temperatures for the month of June and December by retrieving and filtering the required data from the Measurement table in the [hawaii.sqlite](hawaii.sqlite) database.

### Summary Statistics for June and December Temperatures

In this portion of the project, the date column of the Measurement table in the **hawaii.sqlite** database was filtered for retrieving all the temperatures for the month of June and december, the temperatures were then converted to a list and a DataFrame was created from the lists. As a result of this, the summary statitics was generated from the two DataFrames that were created using the **describe()** function for calculating the mean, minimum, maximum, standard deviation and percentiles for both the June and December temperatures DataFrames

Figure below illusrates the summary statistics for the June temperatures DataFrame.

![Summary statitics of temperature for the month of June](Resources/June_temps_summary_statistics.png)


Figure below demonstartes the summary statistics for the December temperatures DataFrame.

![Summary statistics of temperature for the month of December](Resources/December_temps_summary_statistics.png)

The results that can be observed from the summary statstics for the months of June and December are as follows:

- Months of June and December had an average temperatures of **75°F** and **71°F** respectively. This indicates that the daily mean temperatures for each day of the month of June was slightly higher than in December.

- Month of June had a low temperature of **64°F** and high temperature of **85°F**. Whereas December had a low and a high temperatures of **56°F** and **83°F** respectively which indicates that month of June was slightly warmer than December.

- Looking at the **75th** percentiles of **77°F** and **74°F** in months of June and December respectively it is evident that both of these months had relately warm temperature yearly, with June being slightly warmer than December.

- June and December had roughly similar standard deviations of **3.26** and **3.75** respectively. Since the standard deviation for temperatures of both June and December were roughly low this indicates that the temperature did not vary much in both of these months.

## Summary

After performing the required analysis of the temperature trends for the months of June and December in Oahu, Hawaii it was determined that the surf and ice cream shop business seems to be sustainable year-round and it would be a great idea to build the shop in Oahu since both of these months had relatively warm temperature with few variations based on  their **75th** percentile and their relatively low standard deviation.  However, since weather has other attributes such as precipitation, it is a good idea to take this attribute into consideration as well to make sure our data supports opening a surf and ice cream shop completely because there is still a chance that this location might have a rainy weather despite its warm temperature which is another important factor to be taken into consideration for opening a surf and ice cream shop. 

### Summary Statistics for June and December Percipitation

As a result of this additional queries were performed for gathering more weather data for June and December. In addition to temperature, further queries were performed for retriveing the percipiotation data for months of June and December for determining if Oahu has a rainy weather despite its warm temperature. As a result, two additional queries were performed for retrieving the precipitation data from the Measurement table for the months of June and December. The retrieved results were then converted to pandas DataFrame and their summary statistics were generated as shown in figures below.

*Summary statistics of precipitation in June:*

![Summary statistics of precipitation for the Month of June](Resources/June_prcp_summary_statistics.png)


*Summary statistics of precipitation in December:*

![Summary statistics of precipitation for the month of December](Resources/December_prcp_summary_statistics.png)


As it is depicted in the two figures shown above, June had an average of **0.14 inches** percipitation while December had an average percipitation of **0.22 inches**. This indicates that Oahu does not experience heavy rainfalls which is a positive point in addition to its warm weather for builing a surf and ice cream shop. Additionally, a histogram was plotted using the queries and DataFrames created for visualizing the the frequency of percipitation observation in June and December as demonstarted in figures below.

*Precipitation Observation in June:*

![Precipitation observation in June](Resources/June_prcp_histogram.png)

*Precipitation observation in December:*

![Precipitation observation in December](Resources/December_prcp_histogram.png)

Ad it can be seen in the histograms above, the vast majority of the precipitation observations for the month of June is approximately between 0 to 0.5 and between 0 to 0.75 for December. this further concludes that these two months similary experienced moderate to no rain fall. Hence, the achieved results cleary supports opening a surf and ice cream shop as this business seems to be sustainable year-round.