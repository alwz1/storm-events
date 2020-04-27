# Analysis of storm events from 2010 to 2019
### Table of Contents
1. [Installations](#installations)
2. [Project Motivation](#project_motivation)
3. [File Descriptions](#file_descriptions)
4. [Results](#results)
5. [Licensing, Authors, Acknowledgements](#licensing)

### Installations<a name="installations"></a>
Standard libraries installed with the Anaconda distribution.

python 3.7.4

### Project Motivation<a name="project_motivation"></a>
Exploratory data analysis of storm events from 2010 to 2019.
The datasets are from Storm Events Database of National Centers for Environmental Information (NCEI).

1. What are the yearly direct fatalities caused by the top five storm event types?

2. Which storm event types caused the most total fatalities?

3. What are the yearly property damages caused by the top 5 storm event types?

### File Descriptions<a name="file_descriptions"></a>
storm_events.ipynb: Jupyter notebook for EDA of storm events

Storm-Data-Export-Format.pdf: Explanation of data format and field names

LICENSE.txt: MIT License

### Results<a name="results"></a>
The storm events datasets from 2010 to 2019 are downloaded from NCEI database. These csv files are then read and  concatenated into a  pandas data frame. Each yearly dataset contains about 63000 rows and 51 columns. For this project eight features are selected to analyze fatality and damage property. The feature ‘EVENT_ID’ is used to make sure that duplicate events are not included in the analysis. There are 56 storm types. 

I first checked which types occurred most frequently, and found thunderstorm wind, hail, winter weather, flash flood, and drought to be the five most frequent events. However, these most frequently occurring events are not necessarily the most impactful in terms of fatality and property damage. 

Next, I analyzed the fatality. The datasets contains direct and indirect fatality by the storm events. There are no missing values for the fatality in the datasets. To help with the analysis, I created a function called ‘fatality’ that takes a column’s name and returns direct, indirect and total fatality grouped by that column’s name. For example fatality(‘EVENT_TYPE’) returns direct, indirect, and total fatality grouped by EVENT_TYPE. 

The top five storm types that cause the most <b>direct fatality</b> are <b>tornado, flash flood, excessive heat, heat, and rip current</b>. The peak direct fatality of 858 occurred in 2011, and 553 of them are caused by tornados. The median of the yearly direct fatality by tornado is 42. 5. The cumulative percentages of direct fatality are calculated to create a Pareto chart. It is found that these five storm types account for about 60% of direct fatality by all storm events. 

Storm events have significant indirect fatality. For example, winter weather has 56 direct fatalities and 498 indirect fatalities. This is in contrast with rip current that has 489 direct fatalities and 7 indirect fatalities. Because of the difference in indirect fatality, the list of the top five storm types for the <b>total fatality</b> are different from that of direct fatality. They are <b>tornado, excessive heat, heat, flash flood, and winter weather</b>. These storm types account for about 50% of total fatality. 

Next I analyzed the property damage. The property damage are given in K, M or B: 10.00K = $10,000; 10.00M = $10,000,000, and etc. I created a function that converted these strings into numeric property damage in billions by using a dictionary and casting the strings into floats. 

About 18% of property damage values were missing. The median of property damage for each of 56 storm event types was first computed, and the missing values were imputed with the corresponding median values. The medians were used instead of the means because there were great outliers for many of these storm types. For example the median of the property damage for flash flash is zero while the maximum is 10 billion. 

There were 36 storm events that caused one billion dollars or more in property damage. The total property damage caused by these 36 storms was 115.75 billion dollars which is 53% of total property damage by all storm events. 

The top five storm types that caused the most <b>property damage</b> are <b>flash flood, wildfire, flood, tornado, and coastal flood</b>. These storm types caused about 75% of total property damage by all storm types. Flash flood caused more than sixty-three billion dollars in property damage in 2017 alone.

### Licensing, Authors, Acknowledgements<a name="licensing"></a>
MIT License

Storm Events Database from National Centers for Environmental Information. 

The datasets can be found [here](https://www1.ncdc.noaa.gov/pub/data/swdi/stormevents/csvfiles/).
