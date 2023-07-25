[<<< Previous](h.md) | [Next >>>](j.md)  

# Part 9: Overlay Layers

Now that you've learned how to build and apply filters, it's time to begin assembling datasets that will allow you to analyze county-level population growth in the Indiana between 1940 and 1950.

To analyze county-level population growth in the Indiana between 1940 and 1950, you'll begin by creating two feature layers for Indiana Counties in 1940 and 1950. To do so, you'll use the filter tool, two new tools called **overlay layers** and **extract data**, and the State Boundaries feature layer to create versions of the 1940 US County Boundaries and 1950 US County Boundaries feature layers displaying **only** Indiana counties.

### Step 1: Add Relevant Data to the Map Viewer

Begin by adding the following layers to the Map Viewer:
1. State Boundaries
2. 1940 US Counties
3. 1950 US Counties

### Step 2: Filter State Boundaries for Indiana

Before learning how to use **overlay layers**, you first need to create a filtered version of State Boundaries in the Map Viewer that displays only the state of Indiana.

Navigate to the filter tool. Then, build and apply a filter to create the filtered version of State Boundaries displaying Indiana.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2064.jpg">
</p>

After applying your filter, your Map Viewer should look like this:

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2065.jpg">
</p>

### Step 3: Run Overlay Layers

Overlay layers is a tool that allows users to create a new feature class based on a defined spatial relationship (interesect, erase, or union) between an input layer and an overlay layer. 

With the filtered version of US Census Regions, you can use the **overlay layers** tool to create feature layers visualizing Indiana counties in 1940 and 1950 based on the spatial relationship between the filtered version of State Boundaries, 1940 US Counties, and 1950 US Counties.

You can access create overlay layers and other operations for geospatial analysis in the analysis tab of the Map Viewer. Begin by clicking on the analysis tab.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2066.jpg">
</p>

Then, navigate to the overlay layers tool in the manage data section of the analysis tab. 

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2067.jpg">
</p>

Whenever you use an analysis tool to perform an operation in ArcGIS Online, the platform will ask you to define a series of **parameters** that provide ArcGIS Online with instructions for the operation.

**Parameter - a specified condition that dictates how an operation is performed.**

ArcGIS Online will ask you to define parameters in a series of steps laid out in a pane on the right-hand side of your browser. For example, the options to set parameters for the overlay layers tool look like this:

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2068.jpg">
</p>

To use overlay layers, you will need to set parameters for:

<table align="center">
  <tr>
    <th>Parameter</th>
    <th>Description</th>
  </tr>
  <tr>
    <td align="center">Input Features</td>
    <td>This is the layer that contains the features you want to create a new feature class from.</td>
  </tr>
  <tr>
    <td align="center">Overlay Features</td>
    <td>This is the layer used to determine what happens to features from the input layer based on <b>(1)</b> the overlay method and <b>(2)</b> how the input layer features overlap with features in the overlay layer.</td>
  </tr>
  <tr>
    <td align="center">Overlay Settings</td>
    <td>Defines how features in the intput layer are transformed.<br><br>There are three overlay types available in ArcGIS Online:<br>
      <ol>
        <li>Intersect: creates a layer containing only features (or portions of features) that overlap with the overlay layer.<br>
        <li>Erase: creates a layer containing only features (or portions of features) that <b>do not</b> overlap with the overlay layer.
        <li>Union: creates a layer containing features that are combinations of overlapping features in the input and overlay layers.
      </ol>
      <b>Check that the output geometry matches the geometry of the input features.</b>
     </td>
  </tr>
  <tr>
    <td align="center">Output Name</td>
    <td>The name of the new feature layer containing the features created through the overlay.</td>
  </tr>
</table>

Configure the parameters in order to create a feature layer representing Indiana counties in 1940. Name your output 1940 Indiana Counties Overlay. If you need help selecting the correct parameters, consult the image below.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2069.jpg">
</p>

Once you have configured the overlay layers parameters, click the run button.

### Step 4: Examine Output Feature Class and Check for Slivers

After running the analysis, ArcGIS Online will immediately add the output feature class to the Map Viewer as a hosted feature layer.

Your output (1940 Indiana Counties Overlay) should look like this:

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2070.jpg">
</p>

When running tools that use spatial relationships to create new feature classes, it's important to examine your output layer for **slivers**.

**Slivers - a small polygon that can appear along the border of other features following operations like overlay layers. Slivers occur when the input and overlay datasets do not have matching geometry.**

The best way to find if there are any slivers in your dataset after running overlay layers is to examine the attribute table. Open the attribute table for 1940 Indiana counties and examine the table for the presence of slivers.

*Hint: Slivers are generally very small polygons, meaning they will likely have an area significantly smaller than the other features in your dataset. Sorting with the Area in Square Miles field (added when the overlay layers tool runs) is a place to identify potential slivers.*

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2071.jpg">
</p>

By looking at the attribute table, you'll notice that 1940 Indiana Counties Overaly has 265 records, even though there are only 92 counties in Indiana. This means that 1940 Indiana Counties Overlay has 173 slivers!

**Note: If you examine the attribute table, you will also notice that the output layer from the overlay layers tool contains all of the fields from the attribute tables of both input layers.**

### Step 5: Filter Slivers

Since we are interested in examining historical population growth in Indiana counties (not counties and slivers), we need to remove the slivers from our output dataset.

To do, you will need to apply a filter for 1940 Indiana Counties and run a tool called **extract data** to create a sliver free version of 1940 Indiana Counties.

Begin by building and applying an expression that will filter 1940 Indiana Counties to show **only the polygons that represent counties.**

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2072.jpg">
</p>

If you check the attribute table after applying an appropriate filter with the Area in Square Miles field, you will notice that the attribute table for 1940 Indiana Counties Overlay now contains the correct number of features.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2073.jpg">
</p>

### Step 6: Extract Data

Next, navigate to the analysis tab and open the extract data tool.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2074.jpg">
</p>

Extract data allows you to create a downloadble version of a feature layer that (1) contains only filtered features and/or (2) contains features present within a defined extent.

To use extract data, you will need to set parameters for:

<table align="center">
  <tr>
    <th>Parameter</th>
    <th>Description</th>
  </tr>
  <tr>
    <td align="center">Input Layer</td>
    <td>This is the layer that contains the features you want to extract.</td>
  </tr>
  <tr>
    <td align="center">Extent Layer</td>
    <td>Extract data will only extract features that are located within the geometry of the extent layer.<br><br>When extracting a layer with the help of the filter tool, do not specifify an extent layer.<b></td>
  </tr>
  <tr>
    <td align="center">Output Data Format</td>
    <td>This allows you to control the file format of the output containing the extracted features.</td>
  </tr>
  <tr>
    <td align="center">Result File Name</td>
    <td>The name of the new file containing the extracted features.</td>
  </tr>
</table>

Adjust the parameters for the extract data tool to create a shapefile of the filtered, sliver-free version of 1940 Indiana Counties Overlay. Then, run extract data.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2075.jpg">
</p>

### Step 7: Publish 1940 Indiana Counties

After the analysis runs, ArcGIS Online will save the output feature class as a shapefile in the content tab. However, using extract data does not automatically host the new shapefile as a feature layer in ArcGIS Online (unlike with the overlay layers tool).

In order to work with your output feature class, you will need to publish the shapefile as a feature layer via the content tab.

Begin by finding the output feature class in your content tab. Then, click the publish button to publish the 1940 Indiana Counties shapefile as a feature layer.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2076.jpg">
</p>

**Note: "Publishing" a shapefile creates a feature layer only accessible to you, the owner and does not adjust the default sharing permissions.**

### Step 8: View Output Feature Class

After creating a new feature layer from the downloaded shapefile, add the new feature layer to the Map Viewer to examine and work with your extracted data.

When opening the attribute table, you'll notice that the new feature layer has the correct number of features for the quantity of counties in Indiana (92) and contains no slivers.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2077.jpg">
</p>

<p>&nbsp;</p>

> ### Exercise 8: Create 1950 Indiana Counties
> 
> **Task: Create a new feature layer representing Indiana counties in 1950.**

<p>&nbsp;</p>

[<<< Previous](h.md) | [Next >>>](j.md)  
