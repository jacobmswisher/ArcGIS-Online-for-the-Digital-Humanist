[<<< Previous](b.md) | [Next >>>](d.md)  

# Part 3: Gathering Spatial Data

Now that you have taken some time to explore the [Map Viewer](https://notredame.maps.arcgis.com/apps/mapviewer/index.html) and ArcGIS Online's file storage system, it's time to start working with some data! In this section of the workshop, you will learn how to get data into the Map Viewer through two methods:
1. [Searching for available data through ArcGIS Online](#method-1-searcing-for-data-with-arcgis-online)
2. [Importing data into ArcGIS Online via files uploaded from your computer](#method-2-importing-data-to-arcgis-online-with-the-content-tab)

## Method 1: Searcing for Data with ArcGIS Online

As the saying goes, work smarter, not harder. This philosophy applies in the world of GIS where, luckily for you, thousands of universities, government agencies, and individual people have already created many different datasets and made them available to the public. Additionally, through your organizational account, you also have access to ESRI's [Living Atlas](https://livingatlas.arcgis.com/en/home/) which contains various large datasets curated by ESRI. 

When working with GIS data, its always a good idea to determine if somebody else has already created the thing you need for your project and to save yourself considerable amounts of time by not having to create datasets on your own. One of the strengths of ArcGIS Online's Map Viewer is the ability to search for layers in the Living Atlas as well as those published by other ArcGIS Online users.

### Step 1: Navigate to the Add Layer Function and Set Your Search Parameters

To start searching for spatial data with the Map Viewer, navigate to the add layer function by clicking on the layers button on the left-hand taskbar. Then, click the add layer button.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%209.JPG">
</p>

After clicking the add layer button, you will have the option to search for layers on the left-hand side of your browser. At the top of the add layer tool, ArcGIS Online allows you to change your search parameters to one of the following options in order to help you find the data you need for your project:

#### <p align="center">Table 1. Data Search Parameters in ArcGIS Online.</p>
<table align="center">
  <tr>
    <th>Category</th>
    <th>Effect</th>
  </tr>
  <tr>
    <td align="center">My Content</td>
    <td>Limits your search to only include content items you own</td>
  </tr>
  <tr>
    <td align="center">My Favorites</td>
    <td>Limits your search to only inlude content items you star as a favorite. You can manage this in the content tab or by clickking on a layer in the Map Viewer.</td>
  </tr>
  <tr>  
    <td align="center">My Groups</td>
    <td>Limits your search to only include content items assigned to a defined group of users. You can manage groups in the groups tab of ArcGIS Online and manage sharing permissions in the content tab.</td>
  </tr>
  <tr>  
    <td align="center">My Organization</td>
    <td>Limits your search to only include content items published at the organization level. This is a publication setting configured in the content tab that shares a dataset with all users who you have accounts with your organization (ex. University of Notre Dame users).</td>
  </tr>
  <tr>
    <td align="center">Subscription Content</td>
    <td>Allows you to search content for which your organization has a paid subscription.</td>
  </tr>
  <tr>
    <td align="center">Living Atlas</td>
    <td>Limits your search to only include content items that are part of ESRI's Living Atlas</td>
  </tr>
  <tr>  
    <td align="center">ArcGIS Online</td>
    <td>Allows you to search for all datasets made available to everyone on ArcGIS Online. You can set your content to the everyone sharing permission in the content tab.</td>
  </tr>
</table>

**Note: If you haven't worked in ArcGIS Online before, the My Content search parameter will not show any content. This will change once you create your own content later in the workshop.**

For your first search with ArcGIS Online, adjust your parameters to search the Living Atlas using the dropdown menu at the top of the add layer tool.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2010.JPG">
</p>

Next, search for World Countries, a feature layer hosted by ESRI.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2011.JPG">
</p>

### Step 2: Evaluate Your Search Results

Before you add a layer created by a third party to your Map Viewer, it's important to take a moment to evaluate the dataset for its quality. In ArcGIS Online, the best way to do this is to take a look at the **metadata** for a layer.

**Metadata** - Data about data. The set of data attached to a layer or other piece of content that provides information about that dataset.

To look at the metadata for World Countries, click on the hyperlinked title of the feature layer.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2012.JPG">
</p>

As you read through the metadata for World Countries, what do you notice about it? Does this stirke you as a thoroughly-documented dataset? Is there anything you think is missing from the description?

Just as you would evaluate other sources of information, checking the metadata associated with layers available online is a good first step to make sure that the data you have found is (1) appropriate for your project and (2) from a reliable source.

### Step 3: Add Data to the Map Viewer

Now that you have examined the metadata for World Countries, it's time to add the layer to your Map Viewer. You can add World Countries to the Map Viewer in two ways: using the add button in the seach results or clicking the add to map button that appears at the bottom of the screen when viewing the World Countries metadata.

Go ahead and add World Countries to your Map Viewer.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2013.jpg">
</p>

Congratulations! You have succesfully added your first layer to the Map Viewer! Your Map Viewer should look like this:

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2014.JPG">
</p>

### Step 4: Take a Second Look at the Data

Once you have added World Countries to the Map Viewer, its time to take a closer look at the features in the dataset. In addition to reviewing the metadata for a layer, examining the **attribute table** is another way to assess the datasets you find via ArcGIS Online or elsewhere on the internet.

**Attribute table** - A tabular representation of information associated with a feature class. An attribute table is composed of **records** and **fields**.

Each **record** (or row) in the attribute table corresponds to a feature in the feature class.

Each **field** (or column) in the attribute table corresponds to an attribute (a category of information) that is assocociated with each feature in the feature class.

To open the attribute table for World Countries, navigate to the layers tab on the left-hand side of the Map Viewer and click the three-dot options button on the right-hand side of the World Countries layer. Then, click the show table button.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2015.JPG">
</p>

Take a look at the attribute table for World Countries. Can you answer the following questions?
1. How many features are in the feature class World Countries? *Hint: What is a record?*
2. How many attributes are associated with each feature in World Countries?

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2016.JPG">
</p>

Examining a feature class's attribute table is not only a way to figure out what kind of information is associated with the features in the feature class but can also be a method for assessing the reliability of a dataset. Always look in the attribute table to determine whether the data appears **clean**.

**Clean data** - data that has been checked for accuracy (ex. fixing spelling errors).

### Step 5 (Optional): Stylize World Countries

At this point, you may be wondering how to change the **symbology** of layers in ArcGIS Online.

**Symbology** - The visual characteristics of mapped features, including color, icon, outline, etc.

You can adjust using the styles tool on the right-hand toolbar. We will cover symbology in greater detail in [Part 5](e.md) of this workshop.

<br>
<p align="center">
  :rotating_light: :rotating_light: :rotating_light: <b>CAUTION! SAVE YOUR MAP!</b> :rotating_light: :rotating_light: :rotating_light:
</p>
<br>

Before we move on to importing data into ArcGIS Online with the content tab, take a moment to stop and save your map using the save and open button on the left-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2017.JPG">
</p>

Saving a map creates a copy of the map in your content tab that you can reopen, update, and save for future use.

**It is incredibly important that you save your work frequently. ArcGIS Online currently does have an autosave feature. If you close the the Map Viewer tab in your browser and forget to save, you will lose your work.**

<p>&nbsp;</p>

> ### Exercise 1: Practice Searching for Layers with ArcGIS Online
> 
> Now that you have gone through the process of finding the World Countries layer, adding it to the Map Viewer, and saving your map, take some time to explore the incredible trove of data available on ArcGIS Online. 
> 
> **Task: Using the Living Atlas or ArcGIS Online search paramaters, find and add three datasets that interest you to the Map Viewer.**

<p>&nbsp;</p>

## Method 2: Importing Data to ArcGIS Online with the Content Tab

Though there are thousands of datasets published on ArcGIS Online, you can't always find what you are looking for using the platform's search function. Sometimes, users need to bring spatial data they have acquired elsewhere into ArcGIS Online for analysis by importing data through the content tab.

### Step 1: Find the Data You Want to Import

GIS data is often readliy accessible on the internet, especially in the case of data that comes from government sources. Today, we'll practice importing spatial data into ArcGIS Online by finding a feature class for historical railroad lines in the United States. For this execercise, we are going to import a feature class that visualizes the U.S. railroad system in 1861 called RR1861.

Start by navigating to the [Railroads and the Making of Modern America](https://railroads.unl.edu/resources/), a database maintained by the University of Nebraska Lincoln that provides GIS data related to nineteenth-century U.S. railroads.

Data clearinghouses are common platforms through which entieties like UNL host geospatial data available for public use and are an excellent source of different kinds of data for GIS projects.

Once you have navigated to the Railroads and the Making of Modern America site, click on the red link to download the **Historical GIS Shapefiles** file folder. [If you are having trouble finding the link, click here](https://railroads.unl.edu/shared/resources/USrailshps.zip).

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2018.jpg">
</p>

After clicking the link, your computer will download a compressed (zipped) file fold called USrailshps.zip. USrailshps.zip contains shapefiles for the U.S. railroad system for the years 1840, 1845, 1850, 1861, and 1870. To access the shapefiles, begin by uncompressing (extracting) USrailshps.zip to a location of your choice on your computer.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2019%20Windows.jpg">
</p>

Then, navigate through the directory to RR1861. You'll notice that inside RR1861 are a series of files. Together, these files constitute a shapefile, a common file format for storing and sharing GIS data.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2020.jpg">
</p>

To upload RR1861 to ArcGIS Online, create a compressed (zipped) version the file folder containing all of the component parts of the RR1861 shapefile. To do so, select all of the RR1861 folder containing the component parts of the RR1861 shapefile, right click, then click compress to zip file.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2021.jpg">
</p>

**Note: [If needed, click here to download compressed copy of RR1861.](https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Data/RR1861.zip).**

### Step 2: Upload Your Data

Now that you have created a zipped version of the RR1861 feature class, it's time to import RR1861 into ArcGIS Online via the Content Tab.

**Note: ArcGIS Online can create feature layers from many file formats. [Click here for a complete list of file types useable with ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/reference/supported-items.htm).**

To upload RR1861 to ArcGIS Online, navigate to the content tab and click on the new item button on the upper-left-hand side of the browser.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2022.JPG">
</p>

Then, either drag and drop the zipped RR1861 folder into the new item window or click the your device button to open the zipped folder containing RR1861.

When you add the zipped RR1861 folder to the new item window, ArcGIS Online will provide you with a few options to manage how the file is added to your Content Tab:

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2023.jpg">
</p>

Make sure ArcGIS Online has identified the item type for the zipped RR1861 folder as a shapefile, then choose the option to add RR1861.zip and create a hosted feature layer and click next.

Before ArcGIS Online saves the feature class to your Content Tab, the platform will provide you with an opportunity to change the name of the feature class, assign the feature class to a file folder, add tags (which can help you effeciently search through your content), and add initial metadata to the file.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2024.jpg">
</p>

Edit the information in these categories as you see fit. Then, click the save button.

After saving your upload, ArcGIS Online will immediately take you to the page for that content item. Here, you can edit the metadata, sharing permissions, and other elements of the RR1861 feature layer.

### Step 3: Add Your Imported Data to the Map Viewer

Now that you have uploaded the RR1861 shapefile into ArcGIS Online as a feature layer, its time to take a look at your dataset!

Head over to the Map Viewer and add RR1861 to your map. You will find your layer under the My Content section of the add layer tool.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2025.jpg">
</p>

Congratulations! You have successfully uploaded spatial data to ArcGIS Online!

<p>&nbsp;</p>

> ### Exercise 2: Uploading Data
> 
> On your own, take some time to browse the internet and find some GIS data that interests you. A good way to begin is by hopping on your favorite search engine, and searching for a GIS data related to your topic of interest (ex. history GIS data).
> 
> **Task: Find two datasets online and upload them to ArcGIS Online.**
> 
> If you are struggling to find data via a search engine, consider exploring one or more of these data sources to complete this exercise:
> 1. [The China Historical Geographic Information System](https://chgis.fairbank.fas.harvard.edu/)
> 2. [Atlas of Historical County Boundaries](https://digital.newberry.org/ahcb/downloads/index.html)
> 3. [Ancient World Mapping Center](http://awmc.unc.edu/wordpress/map-files/)
> 4. [National Historical GIS](https://www.nhgis.org/) (requires free account creation to access data)

<p>&nbsp;</p>

[<<< Previous](b.md) | [Next >>>](d.md)  
