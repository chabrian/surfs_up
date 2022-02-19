# Surfs Up

## Overview of Surfs Up Analysis

In this project, I have been tasked with analyzing temperature and precipitation weather data for an upstart ice cream shop in Hawaii. The ideal location for an ice cream shop has relatively warm data, prompting surfers and tourists to visit the ice cream shop, but also relatively little precipitation compared to other potential locations. The weather data provided is a compilation of temperature and precipitation measurements from multiple weather stations in the vicinity of a potential location. I collaborated directly with the ice cream shop owner to analyze the data and report the following information:

1. Annual precipitation over the course of a year.
2. Average temperatures over the course of a year.
3. Temperature statistics for June.
4. Temperature statistics for December.

The weather information came in the form of a SQLite database with two tables depicting weather measurements and weather station information. I used Jupyter Notebook and the SQLAlchemy tool to extract data from the database with object-relational mapping (ORM). I then used Pandas and Matplotlib to create dataframes, summary statistics and visualizations for the data. The full set of resources and analysis results are shown below.

## Resources
- Data Sources: hawaii.sqlite
- Software: Python 3, Jupyter Notebook, Flask, SQLite

## Surfs Up Results

The results of this analysis are summarized in the list below.

**Annual Precipitation**
<div align="center">
<img width="674" alt="Precipitation" src="https://user-images.githubusercontent.com/95327115/154815270-15539bf6-89d9-4296-90fa-9b78acdb2aa9.png">
</div>

- This precipitation data shows the amount of rainfall in inches over the course of one year. There appears to be precipitation year round with the most precipitation occuring around August and April.
  
**Annual Temperatures**
<div align="center">
<img width="415" alt="Temperature" src="https://user-images.githubusercontent.com/95327115/154815283-357c274b-de7d-460e-be3b-e47374e2da62.png">
</div>

- The annual temperatures are grouped into twelve (12) bins and range from the minimum temperature, 60degF, to the maximum temperature, 85degF. The histogram shows that most temperatures throughout the year are between 70 and 80degF which is ideal for ice cream.


**June & December Temperature Summary Statistics**
<div align="center">
  
| ![June_Temp](https://user-images.githubusercontent.com/95327115/154815287-49a01690-35e3-4a05-8532-53e2ddd69808.png) | ![Dec_Temp](https://user-images.githubusercontent.com/95327115/154815293-2f928ada-8e05-47ab-9363-9effdec3022a.png) |
| :---: | :---: |
| June Statistics | December Statistics |

</div>

- The average temperature in June is 75degF compared to average temperature in December of 71degF. This temperature difference is relatively small considering the seasonal difference.
  
- The minimum temperature in June is 64degF compared to the minimum temperature in December of 56degF. This shows that there could be some colder days in December where customers will not be inclined to eat ice cream. On the other hand, there will be few cold days below 60degF in June that would prevent customers from ordering ice cream.
  
- The temperature standard deviation for both months is less than 4degF meaning there will not be too much deviation in temperature above or below the average temperatures for the month. In other words, the temperature will reliably be consistently in the 60-70degF range throughout the year.

## Surfs Up Summary

The results of this analysis show that the temperature of this Hawaii location is likely to be consistent throughout the year and will not have a significant impact on the number of customers. There may be some colder days in the winter months, but not enough to deter this location as a potential candidate to open a new store. Since temperature will not effect customers, the seasonal precipitation data may provide more insight into the volume of customers to be expected throughout the year. The following statistic summaries show the difference in precipitation for June and December:
<div align="center">
  
| <img width="136" alt="June_Precip" src="https://user-images.githubusercontent.com/95327115/154815303-0099a059-fd05-4a64-9cc2-085864e918df.png"> | <img width="135" alt="Dec_Precip" src="https://user-images.githubusercontent.com/95327115/154815318-4c63f3b3-bd93-4f79-94e2-3ae1928bdc85.png"> |
|:---:|:---:|
|June Statistics|December Statistics|

</div>

Almost half the days in December and June appear to have little to no rainfall. It also appears that December has on average almost twice the rainfall as June at 0.21" compared to 0.13", respectively. The standard deviation in December is also greater than in June which means that there could be a higher frequency of days with heavy rainfall. The difference in months could be significant, however, this leads to a discussion whether there may be an even better location in Hawaii where rain is less likely to deter potential customers.
