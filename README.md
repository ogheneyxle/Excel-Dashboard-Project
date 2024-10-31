# Excel-Dashboard-Project

## Table of Content
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Preparation](#data-preparation)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

### Project Overview
In this project, we explored bike sales data for a company from their many subsidiaries across the globe. This dataset contains in-depth information about the customers who patronized from different countries. The aim thus is to display key data in an easy-to-read dashboard through meticulous data analysis for clear visualization.

### Data Sources
Bike Sales Data: The primary data source for this data is the “BikeSales.csv” file, containing detailed information regarding how many bikes were sold.

### Tools
- Microsoft Excel

### Data Preparation
In order to get the data from "raw" to usable, I carried out the following processes;
- Checked for and deleted any duplicates
- Standardized the data; spelling or extra space errors
- Checked for and deleted any black rows

### Data Analysis
The aim of this data exploration is to answer three questions primarily;
- What is the average income of the people who bought bikes and the ones who didn't?
- How much distance does the average person who buys a bike and the one who didn't have to commute?
- What age groups bought more bikes?

To answer these questions, I created pivot tables and an accompanying chart to better represent the information. Through the use of slicers, each of these pivot tables and charts helped to further answer even more queries such as;
- What level of education do our buyers and non-buyers have?
- What region/country do they reside?
- How many kids do they have?

These and more can be easily sourced through further exploration. 

You will notice the "Age Group" column in our data, this did not come with the original data but without it, our results would have been messy and clunky. In order to create this column, I used the IF formula, nestling multiple IFs (not IFS) statements within another in order to create three distinct age groups. the command is as follows;
```Excel
=IF(L2>50, "Old",IF(L2 >= 31, "Middle Age", IF(L2<31, "Adolescent", "invalid")))
```

Finally, pivot tables are a great way of displaying these results but isolated, they tell only parts of the whole story. In order to give a much broader view of the story the data is telling, I created a dashboard where they can be observed, queried and used for further analysis (via slicers).

### Results
From the analysis of the bike sales data, I got the following results;
1. Males bought the highest amount of bikes
2. The males who bought bikes earned more on average than the ones who don't and their female counterparts as well
3. Middle aged people bought more bikes in general, accounting for large chunk of sales data.

### Recommendations
From the analysis and the results thereafter, I have the following recommendations;
1. Tailor ads to be more inclusive of middle-aged female consumers
2. Market biking as a couple activity, ensuring the married males who already buy more bikes can include their spouses as well
3. Since less old people buy bikes, less marketing resources should be focused on selling to that demographic

### Limitations
The intital dataset had quite a few duplicates and some of the data was entered with the assumption that certain abbreviations or symbols would be immediately recognizable, they weren't. After thorough cleaning however, the data was much easier to navigate, analyse and most importantly, visualize.

🃏
