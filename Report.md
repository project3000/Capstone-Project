#  Capstone Report 
## Introduction 

My idea for the Capstone Project is to show that when driven by venue and location data from FourSquare, backed up with open source crime data, that it is possible to present the cautious and nervous traveller with a list of attractions to visit supplementd with a graphics showing the occurance of crime in the region of the venue.

A high level approach is as follows:

The travellers decides on a city location [in this case Chicago]
The ForeSquare website is scrapped for the top venues in the city
From this list of top venues the list is augmented with additional grographical data
Using this additional geographical data the top nearby restaurents are selects
The historical crime within a predetermined distance of all venues are obtained
A map is presented to the to the traveller showing the selected venues and crime statistics of the area.
The future probability of a crime happening near or around the selected top sites is also presented to the user
Who is this solution targeted at
This solution is targeted at the cautious traveller. The want to see all the main sites of a city that they have never visited before but at the same time, for whatever reaons unknown, they want to be able to do all that they can to make sure that they stay clear of trouble i.e. is it safe to visit this venue and this restaurant at 4:00 pm in the afternoon.

Some examples of envisioned users include:

A single white female traveller
An elderly traveller that has had previous back experiences when travelling
There are many data science aspect of this project including:

Data Acquisition
Data Cleansing
Data Analysis
Machine Learning
Prediction
Now that the conference is over the Data Sceintist can explore Chigago and feel much safer.

## Data
In this section, I will describe the data used to solve the problem as described previously.

As noted below in the Further Development Section, it is possible to attempt quite complex and sophisticated scenarios when approaching this problem. However, given the size of the project and for simplicity only the following scenario will be addressed:

Query the FourSqaure website for the top sites in Chicago
Use the FourSquare API to get supplemental geographical data about the top sites
Use the FourSquare API to get top restaurent recommendations closest to each of the top site
Use open source Chicago Crime data to provide the user with additional crime data

## Methodology
Methodology section which represents the main component of the report where you discuss and describe any exploratory data analysis that you did, any inferential statistical testing that you performed, and what machine learnings were used and why.

## Results

Let's review the goals of this project.

The idea for the Capstone Project is to show that when driven by venue and location data from FourSquare, backed up with open source crime data, that it is possible to present the cautious and nervous traveller with a list of attractions to visit supplementd with a graphics showing the occurance of crime in the region of the venue.

A high level approach is as follows:

 The travellers decides on a city location [in this case Chicago]
 The ForeSquare website is scrapped for the top venues in the city
 From this list of top venues the list is augmented with additional grographical data
 Using this additional geographical data the top nearby restaurents are selects
 The historical crime within a predetermined distance of all venues are obtained
 A map is presented to the to the traveller showing the selected venues and crime statistics of the area.
 The future prediction of a crime happening near or around the selected top sites is also presented to the user
So all goals have been achieved except the final one. In this Results and Predictions Section this goal is addressed.

The purpose of this project was to see if crime can be predicted. However, the nature of the dataset, particularly the number of different crimes and the unbalanced nature of the dataset, makes it difficult to predict what crime will predict and when. We can, however, repurpose the Crimes DataFrame by spliting the dataset into two distinct balanced sets and randonly assigning to 0 to represent no crime and 1 to present a crime happening. 

## Discussion and Conclusions
Although all of the goals of this project were met there is definitely room for further improvement and development as noted below. However, the goals of the project were met and, with some more work, could easily be devleoped into a fully phledged application that could support the cautious traveller in an unknown location.

Of the contributing data the Chicago Crime data is the one where more data would be good to have. Also not every city in the world makes this data freely available so that is a drawback.

FourSquare proved to be a good source of data but frustrating at times. Despite having a Developer account I regularly exceeded my hourly limit locking me out for the day. This is why Pickle was used to store the captured data.
