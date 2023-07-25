 [<<< Previous](c.md) | [Next >>>](e.md)  

# Part 4: Creating and Editing Feature Layers

In some cases, you may need to create spatial data for a research project. In ArcGIS Online, you can create new feature layers with point, line, or polygon geometry via the Content Tab and edit those feature layers in the Map Viewer.

ArcGIS Online provides users with two methods to create their own feature layers:
1. Creating a feature layer with point geometry from a .csv (comma-separated values file)
2. Creating a feature layer point, line, or polygon geometry in ArcGIS Online

## Method 1: Creating a Feature Layer from a .csv File

Creating a feature layer with point geometry from a .csv file is a very common data creation method in the digital humanites where we often represent our data as points. Though you can create a point feature layer directly in ArcGIS Online, you the .csv method is preferable when creating and editing a dataset with a significant number of records.

In this exercize, you will create a feature layer representing a six significant sites from the Pacific Theater of World War II using WWII_Pacific_Sites.csv.

### Step 1: Open WWII_Pacific_Battles.csv and Explore the Data Structure

Begin by opening WWII_Pacific_Sites.csv in a spreadsheet editor of your choice (ex. Google Sheets or Microsoft Excel). 

[If needed, head here to download a data folder containing copy of WWII_Pacific_Sites.csv](https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Data/WWII_Pacific_Sites.csv)

Then, take a moment to examine the data structure of WWII_Pacific_Sites.csv. Note the presence of the latitude and longitude fields at the end of the table.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2026.jpg">
</p>

### Step 2: Upload WWII_Pacific_Battles.csv to ArcGIS Online

Next, head to the content tab in ArcGIS Online and upload WWII_Pacific_Sites.csv using the new item button. Check that the option to add WWII_Pacific_Sites.csv as a hosted feature layer is selected before clicking next.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2027.jpg">
</p>

Next, verify that ArcGIS Online has identified the correct field types for each field in WWII_Pacific_Sites.csv. Then, click next.

#### <p align="center">Table 2. Field data types in ArcGIS Online.</p>
<table align="center">
  <tr>
    <th>Field Data Type</th>
    <th>Storeable Range</th>
    <th>Use</th?
  </tr>
  <tr>
    <td align="center">String</td>
    <td>255 characters (default)</td>
    <td>Stores information as text</td>
  </tr>
  <tr>
    <td align="center">Short Integer</td>
    <td>-32,768 to 32,767</td>
    <td>Stores whole numbers</td>
  </tr>
  <tr>
    <td align="center">Long Integer</td>
    <td>-2,147,483,648 to 2,147,483,647</td>
    <td>Stores whole numbers</td>
  </tr>
  <tr>  
    <td align="center">Float</td>
    <td>approximately -3.4E38 to 1.2E38</td>
    <td>Stores numbers with decimal places</td>
  </tr>
  <tr>  
    <td align="center">Double</td>
    <td>approximately -2.2E308 to 1.8E308</td>
    <td>Stores numbers with decimal places</td>
  </tr>
  <tr>
    <td align="center">Date</td>
    <td>mm/dd/yyyy hh:mm:ss AM/PM</td>
    <td>Stores date and time information.<br>Can be sorted chronologically.</td>
  </tr>
</table>

<br>

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2028.jpg">
</p>

Finally, confirm that ArcGIS Online has located the fields containing the geographic information for the location of each record in WWII_Pacific_Sites.csv. Then, finish uploading WWII_Pacific_Sites.csv to ArcGIS Online

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2029.jpg">
</p>

**Note: you can also create point feature layers using addresses as the geographic information in a .csv file. [This process is called geocoding](https://doc.arcgis.com/en/arcgis-online/reference/geocode.htm).**

### Step 3: Examine WWII_Pacific_Sites in the Map Viewer

After uploading WWII_Pacific_Sites.csv to ArcGIS Online as a feature layer, head to the map viewer to examine your new dataset and it's attribute table.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2030.jpg">
</p>

<p>&nbsp;</p>

> ## Exercise 3: Creating a Feature Layer for a Campus Tour
> 
> Notre Dame is creating a self-guided tour of campus and is planning to have a GIS interface that visitors can use to navigate to popular locations on campus and find information about those places. They need a GIS analyst to build a feature layer for the new interface, and you have been asked to create the geospatial data for the project.
>
> **Task: Create a point feature layer from a .csv file that contains features for common tour locations on campus as well as links to information about those features. [Information about stops on the campus tour can be found here.](https://tour.nd.edu/locations/)**

<p>&nbsp;</p>

## Method 2: Creating a Feature Layer in ArcGIS Online

In some cases, you may want to build point, line, or polygon feature layers by creating features directly in the ArcGIS Online Map Viewer. This is a good approach for researchers who need to create lines or polygons, or who are working with small point feature layers.

### Step 1: Create an Editable Feature Layer in ArcGIS Online

To create a new, editable feature layer, navigate to the Content Tab, click the new item button, and select the option to create a new feature layer. 

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2031.JPG">
</p>

Select the option to define your own layer, then click the next button.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2032.jpg">
</p>

For this exercise, we are going to create an editable feature layer that visualizes places on the Notre Dame Campus you visited in the last week using point geometry. 

In the create a feature layer window, assign your new layer a name (ex. NDplaces) and make sure the geometry is set to point layer. Then, click the next button.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2033.jpg">
</p>

Though we won't use these options in this exercise, when creating a new feature layer ArcGIS Online does allow you to build more complex datasets by:
1. **Adding multiple layers to a feature layer.** Using this function creates what ArcGIS Online refers to as a **group layer**, or a feature layer that contains multiple feature classes. Using this tool can be useful when, for example, you want to import a single feature layer that represents a collection of features with different geometries (ex. some features as points and others as polygons).
2. **Adding GPS metadata fields.** Enabling this option automatically generates fields for recording information about GPS recievers used to create new features in the feature layer. ArcGIS Online facilitates data creation with GPS recievers through a separate application called [ArcGIS Field Maps](https://www.esri.com/en-us/arcgis/products/arcgis-field-maps/overview).
3. **Enabling Z-values.** This option allows you to store Z coordinates for features, in addition to the standard creation of X,Y coordinates for each feature. Enable this option if you want to create 3D models or track the elevation of features in ArcGIS Online.

Finally, update the metadata and tags as needed for NDplaces. Then, save the new feature layer.

### Step 2: Add Fields

After creating the NDplaces feature layer, we need to finish setting up the layer before creating new features. This involves two steps:
1. Adding fields (attributes)
2. Making the feature layer "editable"

Let's begin by adding a field (attributes) to the NDplaces feature layer to help document the name of each place.

To add a field, start by clicking navigating to the data tab from the content page for the NDplaces feature layer.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2034.jpg">
</p>

In the upper-right hand corner, use the fields button to switch from the table view to the field list view. Then, click the add button on the left to create the name field.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2035.jpg">
</p>

Next, complete the add field form to create a field that will capture the names of the features in the NDplaces feature class.

*Tip: It's generally a good idea to enable the allow null Values option. Null values indicate that the attribute field for a record has no value. This is different than a field that is empty, which in the case of text (or string) fields, would mean that the field has a value of "", which essentially means "nothing". This will become important later on when we begin working with filters, as some filters will return empty values but will not return null values. More on this in [Part 9: Working with Vector Data](i.md).*

**Note: Clicking on a field name in the data tab will allow you to make changes to the field or, if needed, delete the field from the attribute table.**

### Step 3: Make the Feature Layer Editable

After creating fields for your new feature layer, you need to make sure that the feature layer "editable" before you can create new features. Editing settings are managed in the settings tab for your feature layer.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2036.jpg">
</p>

Navigate to the settings tab for NDplaces. Then, scroll down the page until you find the editing settings.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2037.jpg">
</p>

Confirm that the enable editing box is checked and that NDplaces allows all kinds of editing (Add, Delete, Update) for both attributes and geometry. If you needed to change any settings, you will also need to save your changes at the bottom of the page. Save if needed and then navigate back to the overview tab for NDplaces.

*Tip: The editing settings also allow you to manage how collaborators can interact with your feature layer. These settings can be helpful for managing group work on GIS projects.*

### Step 4: Update Metadata

If needed, update the metadata (description, terms of use, etc.) for NDplaces.

### Step 5: Create New Features

Now that you have completed the process of creating an editable feature layer, its time to head back to the Map Viewer and create new features for historical places on campus!

Begin by navigating to the Map Viewer and adding NDplaces to the map (you can do this quickly by clicking the open in Map Viewer button at the top-right of the overview tab).

Once you are in the Map Viewer, open the editor tool by clicking the edit button on the right-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2038.jpg">
</p>

The editor tool allows you to create, edit, and delete features in a feature layer. You can create features by clicking the new feature button and can edit or delete features via the select button (editing after we create our first feature). The filter types function comes into play when editing group layers.

*Tip: Snapping is a setting that, when enabled, automatically connects (snaps) a new edge or vertex of a feature to an existing edge or vertex of another feature when the new edge/vertex is created next to the old one. This feature is particularly useful when creating new polygons, as it ensures that you eliminate empty space (known as a sliver) between polygon features that are supposed to share edges.*

Click the new feature button to start creating your first feature.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2039.jpg">
</p>

After you click the new feature button, your cursor will transform into a data creation tool allowing you to create a new point feature by clicking anywhere on the map. We are going to start by creating a point for the Hesburgh Library at the University of Notre Dame in South Bend, Indiana.

Zoom in on the map, find the Hesburgh Library, and click on the center of the library to create a new point feature. After clicking on the map, a pane will appear on the right side of the browser where you can populate the fields for the new feature. Populate the fields with the name of the feature and today's date and time (*Hint: Hitting tab after entering the date will automatically populate the time with your local time*). Then, click the create button to finish creating the feature.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2040.jpg">
</p>

**Note: After creating a new feature, ArcGIS Online will allow you to keep creating additional features in the Map Viewer until you exit the create feature tool.**

Congratulations! You have succesfully created a new feature in ArcGIS Online. If you want, you can open the attribute table for NDplaces to look at the attribute information for the feature.

### Step 6: Edit Features in the Feature Layer

The editor tool also allows you to edit and delete existing features in a dataset. We'll learn about both functions by editing, then deleting the Hesburgh Library point from the NDhistory.

To edit and delete features, click the select button in the Editor tool.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2041.jpg">
</p>

Then, click on the point for the Hesburgh Library to manage the feature. Let's practice editing the feature by adjusting the date visited field. Change the name to reflect the building's full name, the Theodore Hesburgh Library. Then, click the update button to save your changes.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2042.jpg">
</p>

### Step 7: Delete Features in the Feature Layer

To delete a feature from a feature layer, repeat the process from [Step 6: Edit Features in the Feature Layer](#step-6-edit-features-in-the-feature-layer). However, instead of updating the feature in the edit feature tool, simply click the delete button at the bottom of the pane to delete the selected feature. After deleting the feature, you will be asked to confirm that you want to delete the feature as a deletion is irreversible in ArcGIS Online.

Go ahead and delete the point for the Hesburgh Library now.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2043.jpg">
</p>

**Note: ArcGIS Online automatically saves creations, edits, and deletions for feature layers.**

<p>&nbsp;</p>

> ### Exercise 4: Creating Feature Layers in ArcGIS Online
> 
> **Task: Add at least one new field to NDplaces and create five new point features for places you have recently visited on campus.**
> 
> **Alternatively, create a new feature layer with point, line, and/or polygon geometry in ArcGIS Online using the Content Tab. Choose whatever theme you want for your layer or, alternatively, create a layer with random features. Try to include at least five features > and at least two attribute fields in your dataset.**

<p>&nbsp;</p>

[<<< Previous](c.md) | [Next >>>](e.md)
