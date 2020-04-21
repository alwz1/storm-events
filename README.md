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

1. Which storm events occured most frequently?

2. Which storm events caused the most total fatalities?

3. Which storm events caused the most direct fatalities and what are the yearly fatalities? 

4. Which storm events caused the most property damage and what are the yearly property damage? 

### File Descriptions<a name="file_descriptions"></a>
storm_events.ipynb: Jupyter notebook for EDA of storm events

Storm-Data-Export-Format.pdf: Explanation of data format and field names

LICENSE.txt: MIT License

### Results<a name="results"></a>
The storm events datasets from 2010 to 2019 are downloaded from NCEI database. 
The datasets are concatenated into a dataframe.
There are 56 storm event types. 
The datasets contain direct and indirect fatalities, and property damage in K, M, and B (thousand, million, billion dollars).

The five most frequent events are thunderstorm wind, hail, winter weather, flash flood, and drought.

The storm events that caused the most total fatalities are tornado, excessive heat, heat, flash flood, and winter weather. 

The events that caused the most direct fatalities are tornado, flash flood, excessive heat, heat, and rip current. 
Tornado caused the direct fatalities of 553 in 2011, and flash flood caused the direct fatalities of 142 in 2015.

The events that caused the most property damage are flash flood, wildfire, flood, tornado, and costal flood. 
Flash flood caused the property damage of more than 63 billion dollars in 2017, and wildfire caused the property damage of more than 18 billion dollars in 2018. Costal flood in 2012 caused the property damage of more than 21 billion dollars.

### Licensing, Authors, Acknowledgements<a name="licensing"></a>
MIT License

Storm Events Database from National Centers for Environmental Information. 

Bulk Data Download (CSV)
