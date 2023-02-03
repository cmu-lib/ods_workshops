---
layout: default
grand_parent: Cleaning Untidy Data with OpenRefine
parent: Part 1 OpenRefine Basics with Personal Consumption Expeditures Data
has_children: false
nav_order: 5
title: Transposing data
---

## Transpose the data from wide format to long format


![Transpose set up image](/Users/cmu_lib/portfolio_workshop/OpenRefine_materials/fig/transpose_setup_image_openrefine.jpg)

**Note:** For each state, for each expenditure type, we now have 8 separate rows, one for each year. Notice the dataset now has 9792 rows, compared to 1227 before transposing. It has fewer columns, but many more rows – this is why it is referred to as a “long” format. Long format can be useful for certain types of data analyses, where all your data measuring the same thing (e.g., per capita expenditures) need to be in one column instead of spread over many.