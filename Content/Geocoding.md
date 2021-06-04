---
layout: default
title: Geocoding
nav_order: 4
---

# Geocoding

Open the notebook titled "Geocoding with Python" and run through the steps below.  Refer to the video at the bottom of the page for help.

## Step 1)

Import the necessary packages and read the data file.  Copy the apikey you accessed on the last page and paste it in the first code block of the Geocoding with Python.ipynb where you see:
```python 3
api_key = ""
```

## Step 2)

Inspect the data.  1) Get the count of the total number of records. 2) Aggregate the data by department and sort it.

### Question 1)
How many incidents are there in the datasets?
<!-- 147 -->

### Question 2)
What do the total incidents by department tell us about the nature of police violence in British Columbia?
<!-- RCMP are far and away responsible for the most, followed by BC and Victoria.  A number of incidents occurred at prisons across the province as well. -->

## Step 3)

Aggregate the data by cause of death and plot it.

### Question 3)
What is the most common cause of death during an interaction with police?  What information can you draw from this chart?
<!-- Shootings are most common -->


## Step 4)

Geocode the addresses.

### Question 4)
Did the geocoder fail to recognize any of the locations?
<!-- No -->


## Step 5)

Inspect the results.  Create a web map to display the points.

### Question 5)
What spatial patterns stand out in the data set to you?
<!-- Densest concentration in metro Vancouver -->

### Question 6)
Change the 'fill_color' parameter to 'red'.  Zoom to any specific area/region of interest (eg. Metro Vancouver, Northern BC, etc.).  Take a screenshot and submit it on canvas. 
