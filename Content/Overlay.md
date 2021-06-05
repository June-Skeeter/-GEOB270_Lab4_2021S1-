---
layout: default
title: Vector Overlay
nav_order: 5
---

# Vector Overlay

Open the notebook titled "Vector Overlay with Python" and run through the steps below.  Refer to the video for guidance.

<iframe width="560" height="315" src="https://www.youtube.com/embed/zHVT3Z_WZbs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Step 1)

Import the necessary packages and read the data file. 

## Step 2)

Read the data geocoded text file and covert it to a spatial data format.  This step is equivalent to "display xy data" in ArcGIS Pro.  Then we can quickly plot the data to make sure it imported properly.

### Question 7)
What does looking at the demographics in this data tell you about police involved deaths in Canada?
<!-- Disproportionately male and indigenous but many missing records are a limiting factor.  -->


## Step 3)

Read the Census Subdivision shapefile.  Plot the BC population data to make sure it imported properly.  Plot the point data over polygon layer.

### Question 8)
Zoom to a region of interest and take a screenshot, showing both the points and polygon layer and submit it to canvas.


## Step 4)

Loop through each row in the census subdivision layer.  Do a point in polygon vector overlay using the .within() function to find which incidents are in each polygon.  Add the total number of incidents for each subdivision as an attribute.

### Question 9)
What is the highest number of incidents in a single census subdivision?
<!-- 18 -->


## Step 5)

Normalize the data to calculate the police involved death rate.  Divide the number of incidents by the total population.  First do this for the whole province to calculate the provincial average.


### Question 10)
What is the provincial police involved death rate?
<!-- 3.16 -->

### Question 11)
What does this number mean?
<!-- For every million residents in BC, 3.16 people die from a police interaction per year -->

## Step 6)

Repeat the normalization process for the all census subdivisions.  Then select subdivisions with at least one incident and print the results.

### Question 12)
What is the general pattern you notice in regards to the relationship between the rate, number of incidents, and total population?  What explains this pattern?
<!-- Lower population areas tend to have higher rates.  Partly the small population, causing higher rates.  Partly, the "hidden" nature of police violence in BC.  If Vancouver had a rate as high as these small communities, the issue would get more attention -->


## Step 6)

Repeat the normalization process for the all census subdivisions.  Then select subdivisions with at least one incident and print the results.

### Question 12)
What is the general pattern you notice in regards to the relationship between the rate, number of incidents, and total population?  What explains this pattern?
<!-- Higher rates are in areas with smaller populations.  This is partly an artifact of small samples sizes and partly highlights the hidden nature of police violence in BC -->

## Step 7)

Select just the subdivisions with at least 5,000 residents and plot the relationship between % Indigenous Identity and the Police-Involved Death Rate.  Fix the title so it says the correct years (2011-2021).Then download the plot and submit it to canvas.  
<a href="Download.mp4" target="_blank">See this video instructions for help downloading the plot</a>


Notice the outlier on the plot.  The value in Kent, BC (CSD) is more than double the next highest value. That is because the data from the Georgia Straight includes dearths in prison, and there is a prison in Agassiz, which is in this CSC.

### Question 13)

Submit the plot to canvas.




## Step 8)

Plot the selection as a choropleth map.  

### Question 14)

Change the middle gin value from 10 to 20, then re-run the code block.  Take a screenshot of the map (full scale or zoomed to a specific region) and submit it to canvas.