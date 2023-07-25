[<<< Previous](../README.md) | [Next >>>](b.md)  

# Part 1: Geographic Information Systems - An Overview

This overview provides a brief introduction to Geographic Information Systems (GIS) and some of the important processes and terms you will encounter as your learn more about GIS.

## What is GIS?

**Geographic Information Systems (GIS)** are platforms that store, maintain, and visualize spatial data for use and analysis by users. A GIS can be as simple as a handrawn or printed map and as complex as an application on a mobile phone or software on your computer.

## How does GIS Work?

GIS relies on a process called **projection** to visualize the Earth's surface and to represent **spatial data** on a map.

**Projection** - The process of representing the three-dimensional surface of the earth in a two-dimensional format.

**Spatial data** - Information that exists with an associated geometry and spatial reference.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%201.jpg">
</p>

Earth’s surface can be projected in many ways, each of which distorts objects (such as landmasses) differently. Compare the Universal Transverse Mercator Projection (left) with the USA Contiguous Albers Equal Area Conic (Right). Take note of the size and shape of Alaska. The Mercator is designed for a world map while the Albers is designed for visualizing the continental United States.

**ArcGIS Online uses a version of the Mercator projection called Web Mercator. Users who want to work in different projections will need to choose an alternative GIS platform, though ArcGIS Online can create new datasets for you to download in a projection of your choice.**

## Spatial Data Types

GIS users work with two types of spatial data, **vector data** and **raster data**.

**Vector data** - Spatial data composed of discrete features with a defined geometry (point, line, or polygon). 

Vector data is good for analyzing and displaying data that does not vary within the space occupied by each feature. A vector dataset is referred to as a **feature layer** in ArcGIS Online.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%203.jpg">
</p>

For example, the feature layer above visualizes all of the counties in the state of Kentucky. This feature layer utilizes polygon geometry.

**Raster data** - Spatial data composed of a grid of cells where each cell contains a specified value and multiple cells can have the same value.

Raster data is excellent at displaying change over space. A raster dataset is referred to as a **tile layer** in ArcGIS Online.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%204.JPG">
</p>

This raster is a digital elevation model (DEM) of the state of Kentucky. Each cell has a value for the elevation of the area covered by that cell which allows the GIS software to display continuous changes in elevation across the state. 

**During this workshop, we will only be working with vector data.**

## Vector Data Structure

Vector data is stored as what GIS users call a **feature class**.

**Feature class** - A collection of features that share a **geometry**, common **attribute** fields, and a **spatial reference**.

A **feature class** has three component parts:

1. **Geometry** - Defines how features are represented on a map. Geometry can be one of the following types: point, line, or polygon.
2. **Attribute(s)** - Information about features, such as name, area, etc.
3. **Spatial Reference** - The coordinate system associated with a feature class that allows the GIS platform to match features to their assigned location on the Earth's surface.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%202.jpg">
</p>

You will often hear people refer to feature classes in different ways, such as "layers," "shapefiles," and "feature layers." There is no difference between, for example, a shapefile, and a feature class. Rather, a shapefile *is a type* of feature class stored in a particular file format. 

If you are interested in learning more about GIS file formats, you may consult this [comprehensive list](https://gisgeography.com/gis-formats/).

## What can you do with GIS?

Though we may not realize it, GIS appears regularly in our daily lives. Whether you are working on a research project with spatial data, getting directions on your phone, or wondering how your city manages a schedule of thousands of trash and recycling pickups on a weekly basis, you are engaging with GIS. Like other digital tools, GIS is also increasly becoming an important part of the researcher's toolkit in the humanities and also offers an excellent platform for creating public-facing scholarship with [ArcGIS StoryMaps](https://storymaps.arcgis.com/).

From scholarly applications to professional use in various instutitional settings, the possibilites of what *you* can do with GIS are almost endless!

[<<< Previous](../README.md) | [Next >>>](b.md)  

