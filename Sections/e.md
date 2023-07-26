[<<< Previous](d.md) | [Next >>>](f.md)  

# Part 5: Data Visualization in ArcGIS Online

ArcGIS Online users utilize the styles tool to manipulate the appearance of feature layers in the ArcGIS Online Map Viewer.

In this part of the workshop, you will use the styles and print tools to change the appearance of the RR1861 feature layer and save your data visualization as a map in the format of a .pdf file.

### Step 1: Adjust Feature Layer Symbology

For this part of the workshop, we'll return to working with RR1861. 

Begin by adding RR1861 to your Map Viewer. Then, click the styles tool button on the right-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2044.jpg">
</p>

The styles tool allows you to adjust the symbology of your feature layer. The styles tool uses fields from a feature layer's attribute table to create different data visualizations. As you change the field using the add field button, you'll notice that the style options available to you will change based on the [data type](https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/d.md#table-2-field-data-types-in-arcgis-online) of the chosen field. For a comprehensive list of style options and their associated field data types, consult this [ESRI resource](https://doc.arcgis.com/en/arcgis-online/create-maps/apply-styles-mv.htm).

To begin changing the symbology for RR1861, click the add field button and add the RROWNER1 field.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2045.jpg">
</p>

After adding the RROWNER1 field (field data type: text), you'll notice that the symbology of RR1861 has changed and you have a new style option in the styles tool pane called unique symbols.

Unique symbols changes the color of features to match the data in the selected field (RROWNER1), with each different (unique) entry that appears in the attribute table recieving a unique assigned color.

To adjust to colors assigned using the RROWNER1 field and the unique symbols style, click the style options button.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2046.jpg">
</p>

Style options allows you to further customize your data visualization. Clicking on the edit (pencil) button will allow you to adjust colors, transparency, and feature outlines. Additionally, you can click and drag the various unique symbols to reorder the list of unique features. Reordering the unique symbols list will also reorder the features in the map legend on the bottom-left-hand corner of the Map Viewer if you don't like the default order (unique symbols sorts by the quantity of each unique entry in the attribute table).

Clicking on the three dot button next to the "Other" category will allow you to "move up" features that ArcGIS Online has bucketed under "Other." By default, unique symbols colors features that contain the 10 most-frequent values for the selected field, which in this case is the owner of each rail line. All other features are bucketed under the category of "Other" and are greyed out by default. Selecting the "move up" option will provide each feature with a unique color based on the value that appears in the selected field for the data visualization.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2047.jpg">
</p>

Using the edit tool, adjust the data visualization for RR1861 to your liking. Then, click the done button at the bottom of the styles tool pane to add the new style options to the feature layer.

*Tip: You can adjust whether a legend appears for the selected feature class on your map by clicking the legend button on the left-hand toolbar.*

### Step 2: Adjust the Basemap

In addition to using the styles tool to manage feature layer symbology, it is also important to select and appropriate **basemap** for your data visualization. 

**Basemap** - an imagery layer that usually serves as the backdrop for a map.

To adjust the basemap in the Map Viewer, click the basemap button on the left-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2048.jpg">
</p>

Then, scroll through the basemap options and select a basemap that you think pairs well with RR1861.

Some basemaps allow you to manage the visibility of the reference layer that is part of the basemap. A reference layer provides information about populated places, roads, and other significant features on Earth's surface. However, a modern-day reference map can sometimes feel out of place in data visualizations for the digital humanities, especially for projects that are historical.

If possible, you can manage the visibily of the basemap reference layer by clicking on the current basemap at the top of the basemap selection list. 

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2049.jpg">
</p>

Then, use the eyeball button to turn off the reference layer.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2050.jpg">
</p>

### Step 3: Export Your Data Visualization

After adjusting the symbology for RR1861 and choosing a basemap, it's time to export your data visualization. 

To export a data visualization, click on the print button on the left-hand toolbar in the Map Viewer.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2051.jpg">
</p>

The print tool allows you to export your map in a file format of your choice. Exporting as a layout allows you to include a legend, scale, north arrow, author information, and title with your map. Exporting with the map only option will simply export an image of the map viewer. ArcGIS Online also provides you with the option to manage the quality of your map image (default is 96 dpi) for both export methods.

Click the export button to export a pdf of your map with the default options and then click the link to open the exported file to examine the map layout.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2052.jpg">
</p>

*Tip: Take full advantage of the capabilities of ArcGIS Online by [embedding](https://doc.arcgis.com/en/arcgis-online/share-maps/embed-maps-groups.htm) an interactive version of your data visualization on the web.*

<p>&nbsp;</p>

> ### Exercise 6: Explore the Styles Tool
> 
> **Task: Create a new data visualization using RR1861 or another layer of your choice. Then, export your data visualizations using the print tool.**

<p>&nbsp;</p>

[<<< Previous](d.md) | [Next >>>](f.md)  
