[<<< Previous](g.md) | [Next >>>](i.md)  

# Part 8: Filters

Part of developing a workflow involves determining which computational processes will help you to answer your research question. In GIS, one common method of answering questions that rely on fields in an attribute table is to make a **selection**.

**Selection** - In GIS, the process of selecting features in a feature class that meet certain criteria based on the feature's attributes or location.

In this section of the workshop, you'll learn how to make selections in ArcGIS Online using a tool called **filter**. Later, you'll put this skill into practice as you create data that will allow you to explore county-level population growth in Indiana.

## SQL Expressions
In order to select by attribute in ArcGIS Online, the filter tool uses **structured query language (sql) expressions**.

**SQL Expression** - A combination of fields and conditions that, when applied to a feature layer, return all records (features) that meet the criteria of the expression.

SQL expressesions select features from a feature layer where the information in the selected field meets the specified conditions.

In computational terms, an SQL expression does three things:
1. SELECT features 
2. FROM feature layer 
3. WHERE [Field][Condition][Value]

In an SQL expression, the [Condition] consists of a Boolean Operator (ex. is, and, or, less than, greater than) and a value.

Using the filter tool, you can set the parameters for the [Field] and [Condition] portions of the SQL expression.

Let's practice building and applying a filter in ArcGIS Online with the 1960 US County Population feature layer.

## Step 1: Add Relevant Data to the Map Viewer

Begin by adding 1960 US County Population to the Map Viewer.

## Step 2: Create and Apply a Filter

To apply a filter, begin by clicking on the 1960 US County Population feature layer. Then, open the filter tool using the right-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2059.JPG">
</p>

Next, click the add expression button in the filter tool pane.

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2060.jpg">
</p>

Then, define the parameters for your filter using the filter tool pane. In this case, let's apply a filter that will allow us to determine how many U.S. counties contained at least 100,000 residents in 1960.

Try to create the expression on your own, then check your work using the image below.

**Note: You will notice that different fields allow you to select different operators. This is because certain operators can only be used with certain field data types (ex. you cannot use the "is less than" with a string (text) field.)**

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2061.jpg">
</p>

Then, save the expression to apply the filter to 1960 US County Population.

**Note: If you need to apply a filter to select features that meet multiple criteria, click the add expression button again to build a filter with multiple SQL expressions.**

## Step 3: Open the Attribute Table

After saving the expression, you will notice a visual change in the Map Viewer. When you save a filter, the Map Viewer will hide all of the features that don't meet the parameters of the filter's SQL expression. However, this can't help you figure out the exact number counties with at least 100,000 residents in 1960. 

To view a list and count of the features selected by the filter tool, you'll need to open the attribute table.

As you'll notice, the attribute table has changed to reflect the application of a filter to the feature class. In the attribute table, you can view a list of all selected feature and, by looking at the top of the table, you can determine how many features met the parameters of your selection (303 counties in this case).

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2062.jpg">
</p>

Congratulations! You have succesfully used filters to determine how many counties had at least 100,000 residents in 1960.

*Tip: To remove a filter, retun to the filter tool pane and click the remove filter button.*

<p align="center">
  <img src="https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/Images/Figure%2063.jpg">
</p>

<p>&nbsp;</p>

> ### Exercise 7: Using Filters
> 
> **Task: Using the filters tool and the 1960 US County Population feature layer, answer the following questions.**
> 1. How many counties had a population of less than 10,000 people in 1960?
> 2. How many counties have a name that starts with the letter C?
> 3. How many counties have the same name as the last name of either the first or the sixteenth U.S. presidents?
> 4. How many counties end with the letter N and had a population of less than 50,000 people in 1960
> 5. Which county has a name that starts with D  and had more than 3,300 residents but fewer than 3,500 residents in 1960?
> 
> [Answer Key](https://github.com/jacobmswisher/ArcGIS-Online-for-the-Digital-Humanist/blob/main/Sections/m.md#exercise-7-answer-key)

<p>&nbsp;</p>

[<<< Previous](g.md) | [Next >>>](i.md)  


