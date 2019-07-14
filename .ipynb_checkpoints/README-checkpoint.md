# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project1: Driving Licenses, Traffic Accidents and Casualties Analysis
by Abdullah AlGhamdi

### Overview

In this project, we will make use of tools accumulated so far to gian insighs and draw inferences from provided raw data. The provided datasets:

- [Traffic Accidents and Casualties by Region](/data/saudi-arabia-traffic-accidents-and-casualties-injured-dead-2008.csv)
- [Driving Licenses Issued By Administrative Area](/data/saudi-arabia-driving-licenses-issued-in-the-kingdom-2004-2008.csv)

the dataset will be processed and manipulated using pandas in order to extract plot and charts by using matplotlib and seaborn so we can use our natural pattern recognition to further explore the data and draw proper conclusions. the findings of the project are summerized and presented in [this page](https://caramellaapp.com/private/lEHgw-U1u/l9nDhU6CD/hwadth-altrq-fy-almmlkh-alarbyh-alsawdyh)

### Contents:
- [Datasets Description](#Datasets-Description)
- [Data Import & Cleaning](#Data-Import-and-Cleaning)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Visualization](#Visualize-the-data)
- [Descriptive and Inferential Statistics](#Descriptive-and-Inferential-Statistics)
- [Outside Research](#Outside-Research)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)
- [Blog](#Blog)
## Datasets Description

[Driving Licenses](https://datasource.kapsarc.org/explore/dataset/saudi-arabia-driving-licenses-issued-in-the-kingdom-2004-2008/information/?disjunctive.administritive_area&sort=time_period&location=5,24.37495,45.08024&basemap=jawg.streets)
This dataset contains Saudi Arabia Driving Licenses Issued By Administrative Area for 1993 - 2016. Data from General Authority for Statistics . Follow datasource.kapsarc.org for timely data to advance energy economics research.

[Traffic Accidents and Casualties](https://datasource.kapsarc.org/explore/dataset/saudi-arabia-traffic-accidents-and-casualties-injured-dead-2008/export/?disjunctive.region&disjunctive.indicator&sort=time_period)
This dataset contains Saudi Arabia Traffic Accidents and Casualties by Region for 2016. Data from General Authority for Statistics. Follow datasource.kapsarc.org for timely data to advance energy economics research.

## Data Import and Cleaning

the data is read and stored in a pandas dataframe. A simple check reveals the need for some processing in order to make the data useable. Data cleaning has been carried out according to the following steps:

- find proper deliliter to separate lumped entries properly.
- remove unnecessary characters and/or symbols.
- check datatype and make necessary conversations.
- check for incorrect values such as redundant indeces, typos, and mismatch in names.
- drop unnecessary data.
- check the overall structure of the dataframes and decide whether it needs conversion to/from wide/long format in order to recover its original state.
- merge the dataframes while preserving the most of data.

the two processed datasets are stored in `combined_datasets.csv`. The data content is described in the following table:

|Feature|Type|Dataset|Description|
|:---:|:---|:---:|---|
|**year**|_integer_|Driving_Licenses/Traffic_Accidents|year of issue/occurance | 
|**region**|_object_|Driving_Licenses/Traffic_Accidents|Adminstrative area of Kingdom of Saudi Arabia of issue/where accident took place|
|**indicator**|_object_|Traffic_Accidents|Three classes of accident outcome: the total number of accidents, casualties(dead), and casualties(injured)  | 
|**driving_licenses**|_integer_|Driving_Licenses|number of issued driving liscences|
|**value**|_integer_|Traffic_Accidents|count of class corresponding to _indicator_| 
|**longitude**|_float_|Driving_Licenses/Traffic_Accidents|the longitude of 2d GPS location| 
|**latitude**|_float_|Driving_Licenses/Traffic_Accidents|the latitude of 2d GPS location| 

## Exploratory Data Analysis

The resultant dataframe is explored using pandas _df.describe()_ function to get some descriptive statistics about the data. This will help determining trends and relationships, discover patterns, and spot anomalies in data so it is easier to pick what parts to visualize in the next step.

## Visualize the data

Data is visualized using multiple commands in matiplotlib and seaborn. Using: **a)** insights from descriptive statistics in previous step, and **b)** experimentation with produced plots, we worked on designing plot and charts that best summarizes our findings and illustrates proper inferances.

## Descriptive and Inferential Statistics

with the inferences from the previous two step, we subject the data to further examinations to either extrapolate extra information or decide what additional data could help in that. Some hypotheses we tests, and the result of the test aided us in determining the type pf data to search for.

## Outside Research
[2010 census data](http://www.statoids.com/usa.html) is read into a dataframe. Aided with the new data, we continued working on our inferential statistics. Additionall data helped in making more sense about drawn conclusions.

## Blog
the findings of the project are summerized and presented in [this page](https://caramellaapp.com/private/lEHgw-U1u/l9nDhU6CD/hwadth-altrq-fy-almmlkh-alarbyh-alsawdyh)
