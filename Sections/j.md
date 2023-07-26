[<<< Previous](i.md) | [Next >>>](k.md)  

# Part 10: Table Joins

Now that you have created feature layers representing Indiana counties in 1940 and 1950, it's time to add information about the population of each county to those feature layers so that you can finally analyze population growth in the Indiana between 1940 and 1950.

Currently, the information about each county's population in 1940 and 1950 is in a series of tables:
1. 1940 US County Population
2. 1950 US County Population

To add the information in each .csv to the corresponding feature layer, you will need to learn how to perform an operation called a **join.**

## What are Joins?

A **join** is an operation that appends (joins) information in the attribute table of one dataset (the join dataset) to the attribute table of another dataset (the target dataset).

In ArcGIS Online, you can perform two types of joins:
1. A **table join** - appends information from a **table** (either a standalone table or feature class attribute table) to the attribute table of a **feature class** based on a **relationship between both tables**.
2. A **spatial join** - appends information from the attribute table of one **feature class** to the attribute table of another **feature class** based on a **spatial relationship** between the features in both feature classes.

In this part of the workshop, you will learn how to perform a table join using ArcGIS Online.

## How Table Joins Work

Table joins append information from a table (usually in the form of a .csv file) to the attribute table of a target feature class.

To join information from the table and feature class, the table join operation relies on the presence of a **key field**.

**Key field - a common field present in the tables of both the target and join datasets.**

For example, analysts often use a common name or id field to join two datasets together. In this example, ID serves as the **key field** to join a list of addresses to a list of grocery stores in South Bend.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2078.jpg">
</p>

To see how table joins work in ArcGIS Online, you'll practice by joining the information in the 1940 US County Population table to the attribute table of the 1940 Indiana Counties Feature Class.

### Step 1: Add Relevant Data to the Map Viewer

Begin by adding the 1940 US County Population table and the 1940 Indiana Counties feature layer to the Map Viewer.

To add the 1940 US County Population table to the Map Viewer, use the tables button on the left-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2079.jpg">
</p>

### Step 2: Define Join Parameters in the Analysis Tab

Next, navigate to the join features tool in the summarize data section of the analysis tab.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2080.jpg">
</p>

When using the join features tool, you will need to set parameters for:

<table align="center">
  <tr>
    <th>Parameter</th>
    <th>Description</th>
  </tr>
  <tr>
    <td align="center">Target Layer</td>
    <td>The feature class containing the features you want to join new information to.</td>
  </tr>
  <tr>
    <td align="center">Join Layer</td>
    <td>The dataset containing the information to be appended to the target layer. <b>Join layers can be feature layers or tables</b></td>
  </tr>
  <tr>
    <td align="center">Join Settings</td>
    <td>Identifies whether the operation is a <b>table join</b> ("use attribute relationship") or a <b>spatial join</b> ("use spatial relationship").</td>
  </tr>
  <tr>
    <td align="center">Join Operation</td>
    <td>Defines how the the join layer is appended to the target layer.<br><br><b>Join one to one</b> matches each record in the join layer to a single record in the target layer while <b>join one to many</b> matches each record in the join layer to every matching record in the target layer.<br><br><b>Join one to many</b> is commonly used in spatial joins but can be used with table joins too (ex. joining a list of states to campgrounds where each campground has a state id field which means that many campground records would have a common value in the state id field).<br><br><b>Define which record is kept</b> allows you to control the join in cases when multiple records in one layer would be joined to a single record in the the other layer.<br><br><b>Keep all target features</b> allows you to control which features appear in the output feature class. Check this box if you want to keep all features in the target layer even if not all target layer features would recieve appended information via the join layer.</td>
  </tr>
  <tr>
    <td>Join Type</td>
    <td>Allows you to control whether the output layer will include features from the join layer that do not match a record in the target layer attribute table (left join) or if those unmatched features should be discarded (inner join)</td>
  </tr>
  <tr>
    <td align="center">Result Layer Name</td>
    <td>The name of the new feature class containing the joined features.</td>
  </tr>
</table>

To join 1940 US County Population to 1940 Indiana Counties, configure the parameters for join features so that 1940 US County Population is joined to 1940 Indiana Counties using a one-to-one table join. In this case, the key field for the table join is called GISJOIN. 

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2081.jpg">
  <br>
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2082.jpg">
</p>

### Step 3: Join 1940 US County Population to 1940 Indiana Counties

After configuring the parameters for the join layers tool, click the run analysis button to join 1940 US County Population to 1940 Indiana Counties.

### Step 4: Examine the Output Feature Class

After the analysis runs, open up the attribute table for the ouput feature class containing the joined features. In the attribute table, you'll see that each record for an individual county in 1940 Indiana Counties now has information for the population of that county in 1940.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2083.jpg">
</p>

<p>&nbsp;</p>

> ### Exercise 9: Table Joins
> 
> **Task: Using the join features tool, join the information in 1950 US Population to the attribute table of 1950 Indiana Counties**

<p>&nbsp;</p>

[<<< Previous](i.md) | [Next >>>](k.md)  
