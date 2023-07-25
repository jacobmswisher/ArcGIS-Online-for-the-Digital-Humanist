[<<< Previous](e.md) | [Next >>>](g.md) 

# Part 6: Geospatial Analysis - An Overview

This page provides an overview of geospatial analysis. Here, you can read more about what geospatial analysis is, how geospatial analysis works, and how geospatial analysts approach problem-solving using workflows.

## What is Geospatial Analysis?

Geospatial analysis is a multi-step approach to problem-solving that involves the use GIS software to perform operations on spatial data. 

## How does Geospatial Analysis Work?

Take, for example, the following research question related to the topic of logistics, railroads, and the U.S. Civil War: **how extensive were rail networks in Union and Confederate states at the start of the U.S. Civil War?**

To solve this research problem, a geospatial analyst would begin by gathering data related to the research question. In this case, the analyst would acquire or create a feature class containing in the United States in 1861, like the one availble from UNL's Railroads and the Making of Modern America. By mapping the railroad lines, the analyst would be able to **vizualize** where people had built railroads by start of the U.S. Civil War in 1861. But how could the analyst determine how extensive Union and Confederacy rail networks were in 1861?

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2053.jpg">
</p>

First, since the analyst is interested in Union and Confederate states, they would need to create or acquire feature layers representing the boundaries of Union states and Confederate states during the Civil War.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2054.jpg">
</p>

Then, the analyst could use an operation you will learn about in this workshop called overlay layers to create two new datasets containing the features from RR1861 that existed within the boundaries of the Union states and Confederate states feature layers.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2055.jpg">
</p>

Finally, the analyst could look at the attribute table for each feature new feature class and discover that there were 20, 754 miles of railroads in Union States compared to the 8,735 miles of railroads in Confederate States in 1861.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2056.jpg">
</p>

## Using Workflows

The process outlined above is what GIS analysts refer to as a **workflow**.

**Workflow - a planned, multi-step sequence that combines data and operations to solve answer a question.**

In this case, the workflow for determining how extensive Union and Confederate state rail networks were at the start of the U.S. Civil War looked like this:

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2057.jpg">
</p>

One of the goals of this workshop is for you to become proficient with assembling the different tools you will learn how to use into workflows that will allow you to solve problems and answer questions using ArcGIS Online. However, there is not always a **right** workflow for solving a problem. Rather, developing workflows is often about making choices that **feel right to you** in order to effectively combine operations and spatial data to answer a research question.

[<<< Previous](e.md) | [Next >>>](g.md) 
