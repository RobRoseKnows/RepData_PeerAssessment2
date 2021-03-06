# Public Health and Economic Consequences of Severe Weather Events in the United State(1950-2011)
Created by Keshav Seth  
Friday 23 January 2015  
##Introduction
_ _ _
Storms and other severe weather events can cause both public health and
economic problems for communities and municipalities. Many severe events can
result in fatalities, injuries, and property damage, and preventing such
outcomes to the extent possible is a key concern.

This project involves exploring the U.S. National Oceanic and Atmospheric
Administration's (NOAA) storm database. This database tracks characteristics of
major storms and weather events in the United States, including when and where
they occur, as well as estimates of any fatalities, injuries, and property
damage.

_ _ _

##Synopsis
_ _ _
In this report, we aim to analyze the impact of different weather events on
public health and economy based on the storm database collected from the U.S.
National Oceanic and Atmospheric Administration's (NOAA) from 1950 - 2011. We
will use the estimates of fatalities, injuries, property and crop damage to
decide which types of event are **most harmful** to the population health
and economy.

This analysis on storm event database revealed that *tornadoes* are the
most dangerous weather event to the *population health*. The second most
dangerous event type is the excessive heat. The economic impact of weather
events was also analyzed. *Floods* and *thunderstorm winds* caused
billions of dollars in property damages between 1950 and 2011. The largest crop
damage caused by drought, followed by flood and hails.

_ _ _

##Data Processing
_ _ _
#####Data :
The data for this assignment come in the form of a comma-separated-value file 
compressed via the bzip2 algorithm to reduce its size. You can download the file
from the course web site:

* [Storm Data](https://d396qusza40orc.buttfront.net/repdata%2Fdata%2FStormData.csv.bz2)  [47Mb]

There is also some documentation of the database available.
Here you will find how some of the variables are constructed/defined.

* National Weather Service [Storm Data Documentation](https://d396qusza40orc.buttfront.net/repdata%2Fpeer2_doc%2Fpd01016005curr.pdf)

* National Climatic Data Center Storm Events [FAQ](https://d396qusza40orc.buttfront.net/repdata%2Fpeer2_doc%2FNCDC%20Storm%20Events-FAQ%20Page.pdf)

The events in the database start in the year **1950** and end in November **2011**. In
the earlier years of the database there are generally fewer events recorded,
most likely due to a lack of good records. More recent years should be
considered more complete.

####Load the libraries :
Following are the libraries required in the analysis.

```r
library(plyr)
library(ggplot2)
library(knitr)
library(grid)
library(gridExtra)
```

####Insatantiate data object :
We setup the working directory. You can change the working directory according to the location of your .bz2 file.

```r
setwd("/home/potato_head/DS/5. Reproducible Research/Week 3/RepData_PeerAssessment2/")
```
_ _ _

