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
The storm events datasets from 2010 to 2019 are downloaded from NCEI database. 
The datasets are concatenated into a dataframe.
There are 56 storm event types. 
The datasets contain direct and indirect fatalities, and property damage in K, M, and B (thousand, million, billion dollars).

The top five storm types for direct fatalities are tornado, flash flood, excessive heat, heat, and rip current. Tornados in 2011 caused the direct deaths of 553.

The list of top five storm events for total fatality are tornado, excessive heat, heat, flash flood, and winter weather. This list is slightly different from the direct fatality list because winter weather storm events caused significant indirect fatalities. 

Flash flood caused the most property damage followed by wildfire, flood, tornado, and coastal flood. Flash flood caused more than sixty-three billion dollars in property damage in 2017.


### Licensing, Authors, Acknowledgements<a name="licensing"></a>
MIT License

Storm Events Database from National Centers for Environmental Information. 

The datasets can be found [here](https://www1.ncdc.noaa.gov/pub/data/swdi/stormevents/csvfiles/).
