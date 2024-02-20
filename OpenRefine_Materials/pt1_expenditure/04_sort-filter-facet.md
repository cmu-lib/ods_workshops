---
layout: default
grand_parent: Cleaning Untidy Data with OpenRefine
parent: Part 1 OpenRefine Basics with Personal Consumption Expeditures Data
has_children: false
nav_order: 4
title: Sorting, filtering and faceting
---

## Sort, filter and facet data
1. **Sort data on a row:** Rows of data are initially loaded in the order they appear in the original data file. In this case, they are grouped by state, with Alabama first. To change the sort, from the State column pull down menu, select Sort... In the Sort window, sort as text, ordered from z-a. Click OK.
2. **Add a secondary sort:** From the 2017 column pull down menu, select Sort..., and sort by numbers, from largest first. Notice the “sort by this column alone” option – that only appears when there is already one or more sorts in place. If you don’t check that option, it will keep the original sort and add this as a secondary sort. 
3. **Remove a sort:** You can remove a sort at any time by pulling down the column’s menu, and choosing Sort -> Remove sort. 
4. **Filter the data:** Filtering allows us to search for certain information within our dataset. Let’s say we want to display only the Pennsylvania data. From the State column pull down menu, choose Text filter. The text filter appears in the left-hand sidebar, under the “Facet/Filter” tab. Type 'pennsylvania' in the search box. OpenRefine automatically removes any rows from the display that don’t match, leaving a total of 24 rows remaining (out of 1224 total).
5. **Add a second filter:** We can have text filters on more than one column at a time. From the Expenditure column pull down menu, choose Text filter. Type 'food' in the search box for that filter. The two filters are combined, showing us all the food-related expenditure categories for Pennsylvania.
	* Note that any functions you perform on filtered data will only be performed on the filtered records, not the entire dataset. This is also true of exporting the file--if you have filters applied, only the filtered data will appear in the export.
6. **Remove filters:** You can remove a filter by clicking on the x in the top left-hand corner of the filter box. Remove both filters now. You should have all 1224 rows displayed again.
7. **Creating a facet:**  A facet summarizes all the values that appear in the column, and lets you select which data to view, as well as provides ways to edit the data. From the State column pull down menu, choose Facet -> Text facet. The facet appears in the left-hand sidebar, in the same area where the filters were previously. It shows you how many total values there are in this column (50), how many rows contain each value (for this dataset it is the same for each, 24), and allows you to sort the values by name or by count (count won’t be helpful in this case since they all have the same count).
8. **Filter data using facets:** Click on Pennsylvania in the value list. This has the same effect as using the text filter to search for Pennsylvania, leaving 24 matching rows. However, from there we can do more than the filter allowed. We can select a second value at the same time. Hover your cursor over West Virginia in the value list and choose include. You can then exclude one or both of the selections at any time. Hover your cursor over Pennsylvania in the value list and choose exclude. Now only West Virginia rows are shown.
9. **Working with numeric facets:** From the 2017 column pull down menu, expand Facet, and look at the options. There are some other types of facets available, including numeric facets. If we created a numeric facet now, it would only work for this column, so you would have to facet each year of data separately. Let’s manipulate the data a bit first, and then come back and work with numeric facets.

### Activity 1 
In addition to the text facet on State, add another text facet on the expenditure column. Using the facets, view the Pennsylvania, West Virginia and Ohio data for "Gasoline and other energy goods" expenditures.  Which state spent the most per capita in 2017?

### Bonus Activity 
Remove the above facets. Apply a numeric facet to the 2017 columns and facet to only expenditures over \$30,000. Using an additional facet, determine the expenditure category with the most values over \$30000. 
