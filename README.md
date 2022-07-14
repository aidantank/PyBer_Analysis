# PyBer_Analysis
## Overview
This report aims to detail the differences in ride sharing data from PyBer by city type. Firstly, it will show how total rides, total drivers, total fares, average fare per ride and rdiver, and total fare differ by city type. Then, we will create a line chart plotting total fares over the course of the first five months of 2019 for PyBer to determine how the company can address the discrepancies between urban, suburban, and rural ride sharing fares.

## Resources
- Data Sources: [city_data.csv](/Resources/city_data.csv) and [ride_data.csv](/Resources/ride_data.csv)
- Software: Python 3.7.13, Jupyter Notebook 6.4.8, Anaconda 4.13.0, Visual Studio Code 1.68.1

## Results
### Tabular
The below table is a summary of each type of city (Rural, Suburban, and Urban) by different metrics. 

![](/analysis/Summary_df.PNG)
> *Table 1*

- Total Rides:
    - The total number of urban rides outnumbers both suburban and rural combined. The more urban the city is, the higher the number of total rides.
- Total Drivers:
    - Similarly to total rides, the number of total drivers increases the more urban a city is. Urban once again has more total drivers than suburban and rural drivers combined.
- Total Fares:
    - As one would expect, the more rides, the higher the total fare. Urban cities have over twice the total fares as suburban cities and rural cities make considerably less in total fares.
- Average Fare per Ride:
    - The opposite is true for average fare per ride. The more rural the city is, the higher the average fare. Rural cities have almost $35/ride where as urban cities make just under $25/ride. 
- Average Fare per Driver:
    - This difference is even more stark when looking at average fare per driver. The average rural city driver makes roughly $55 dollars whereas urban city drivers only average around $16. This metric, like average fare per ride, has a negative relationship between average fare and how urban the city is. I suspect this is likely due to the distance each ride is.


### Graphical
In the below figure, the fare by city type is mapped across the first five months of 2019. Each data point takes the sum of all the fares in a given week by the city type. 

![](/analysis/PyBer_fare_summary.png)
> *Figure 1*

As noted in the tabular results, urban cities see a higher fare than suburban which sees a higher fare than rural cities. There are some fluxuations in the weekly fares, but Urban fares are always the highest, and rural fares are always the lowest for a given week. Plotted across five months, you can see it isn't just one week or month that has super high fares. The total fare amount stays consistant for all city types.

## Summary
### Recommendations
After analyzing the data above I have included three recommendations for PyBer to address the disparities between city types.

1. In order to equalize out the average fare per driver and total drivers, try to incentivize urban or suburban drives to switch to rural cities. This way the average fare of each driver by city type would be closer together.
2. The majority of total rides and total fares occur in urban cities. Another suggestion would be to attempt to market to more suburban and rural cities. Increasing the number total rides in rural cites would help increase the total fares in rural cites as they are lagging way behind urban cities in those metrics. 
3. Lastly, if the business is looking to decrease their total number of drivers to increase average fare per driver, I would suggest the urban drivers first. They have the lowest average fare per driver and are the only city type where total drivers outnumbers total rides.

As a final point, I would recommend looking into acquring data for distance traveled by each ride. This would be another important variable for analysis on ride sharing data by city type for PyBer.