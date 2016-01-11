---
layout: page
title: Homework
---

## Homework 1: Data basics (Due: 1/12/2016)

# Problem: 
- Obtain the CSV (comma separated variable) file containing the counts of bicycles crossing the Fremont Bridge since 2012 
(as described [here](https://data.seattle.gov/browse?category=Transportation&limitTo=datasets&utf8=%E2%9C%93)). 
- Create a project directory with subdirectories for data and analysis, and create a README file. 
- Download the data from [here](https://data.seattle.gov/resource/4xy5-26gy.csv). Put the it into the data directory.
- Create an iPython Notebook to analyze these data. In the notebook: (1) Isolate the 2015 data, creating fields for date, hour, and count; 
(2) use python matplotlib to plot the counts by hour;  (3) compute hourly average counts over the year; and (4) determine what is the busiest hour of the day.

# Hints 

- The “date” field is a string coded as “yyyy-mm-dd-Thh” where “yyyy” is the year, “mm” is the month, “dd” is the day, and “hh” is the hour. (You’ll need to write python code to decode the strings.)
- To select data of just a particular year, etc. you can use [Boolean indexing](http://pandas.pydata.org/pandas-docs/stable/indexing.html#boolean-indexing) of the array. For example, in the analysis we did in class you can write

    data2015 = data[times.year == 2015]

See the [Pandas indexing documentation](http://pandas.pydata.org/pandas-docs/stable/indexing.html) for more information.
