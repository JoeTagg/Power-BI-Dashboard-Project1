# Power-BI-Dashboard-Project1

## Overview
This project aimed to visualise large data sets relating to Global Land Temperature. It involved cleaning, transforming, querying and analysing data, before displaying and visualising it in an interactive dashboard. More focused on experimenting and displaying Power BI functionality, rather than extracting real-world insights from the data.

## Tools Used
- Kaggle (for original data set)
- Power BI Desktop
- Power BI Service

## Approach/Steps Taken:
- Downloaded 3 x data sets from Kaggle, imported into Power BI Desktop
- Transformed and cleaned each table. Correcting data types, grouping by fields, adding custom columns and DAX
- Loaded and created relationships in Model View between Year and Country fields
- Created new measures for elements like temperature variance, earliest/latest year, temperature of earliest/last year etc.
- Produced all visualisations, based on Global Temperatures, Temperature by Country, Temperature by Major City
- Applied filters where appropriate, formatted, and published

## Key Visualisations
1. Slider: start/end year slicer
2. Cards: ave temp in 1850; ave temp in 2015; % increase; actual celsius increase
3. Line graphs: six major cities displayed showing upward trend in average temperature across time period
4. Bar chart: top 10 countries with the greatest variance/increase of ave temp over time
5. Scatter chart: top 10 countries by average temperature over time
6. Line graph: global average temperature over time
7. Map: sum of average temperature by country, represented by gradient colour
8. Slicer: country slicer

## Improvements
- Given more time there are several improvements and additions that could/should be made
- A year slider connected to the map would provide interesting visuals of temperature changes over time. This would require additional measures and DAX to achieve
- Ideally the scatter graph data point colours would have been displayed vertically darkest to lightest
- Additional visualisations of country temperature changes plotted against global averages would be interesting, to see how much they deviate above/below
- There are a number of interactions and depedencies between visuals that need reworking. They are currently very simplistic
- Continents should be removed from the country slicer list
- Like the major city graphs, but a city/country selection from a drop down list and associated line graph would have been good 

## Caveats
- The original data set, whilst based on real accumulated data, required a lot of cleaning and standardising
- A large number of missing values, especially pre-1850. I took the decision to only focus on 1850-2015 as this provided the most consistent values
- Map visual doesn't yet represent what I'd hoped. It's currently showing the earliest year's recorded temperature, rather than the overall average across all years. By moving the first dial on the year slider at the top, it's possible to get a sense of the changing (increasing) temperatures across geographies.
- There seems to be several anomalies in the data, at least as they are represented in the charts. For example on the scatter chart, there are many outliers recorded in 1862.
- I set myself the challenge of creating this within 48hrs, more focused on learning more of the ins and outs of Power BI, rather than have a fully functioning dashboard that meets a brief
