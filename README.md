# Power-BI-Dashboard

## Overview
This project aimed to replicate a real-world Ecommerce Sales solution. It focused on transforming and analysing transactional data, to then feed into a dynamic dashboard, from which commercial trends/insights etc. could be gained.

## Tools Used
- Kaggle (for original data set)
- Excel Powery Query (to transform and clean data)
- Excel (to create pivot tables, charts, and dashboard)

## Key Queries/Pivots
1. Current YTD total / Previous FY Total / YoY % variance
2. Current YTD total orders / Previous FY total orders / YoY % variance
3. Current YTD total products sold / Previous FY total products sold / YoY % variance
4. Average order value (across all years)
5. Top 10 Products (by total sales across all years)
6. Top 10 Customer IDs (by total sales across all years)
7. Top 10 Countries (by total revenue & relative % of total across all years)
8. Peak Sales by Day of Week (across all years)
9. Peak Sales by Hour of Day (across all years)

## Insights & Trends
1. Data
- Original data required lots of cleaning
- Vast amount of transaction records were not attributed to a customer ID, perhaps they purchased in 'Guest' mode. Worth investigating, as missing out on a large amount of customer buying insights
- Large number of transactions featuring non-standard product descriptions. Perhaps stock transfer, gratis orders, stock balancing. Would need investigation and ideally routing elsewhere
- Significant min/max price distribution for many product lines. Box plot chart can be produced to visual this. Some variance explained by discounts applied at checkout, revenue lost by such variance
2. Visualisations
- Incredibly strong performance and year-on-year growth, across revenue, order volume, and quantity of products shifted
- Average order value remains steady, neglible variance between 2010 and 2011
- No significant month/seasonal buying trends, maybe a small peak and uplift in July
- Good performance and spread of products. Would be worth adding categories/buckets to group products. Analysing such groups might reveal further trends
- CustomerID: 18102 and 14646 vastly outspend (c.£135k and c.£85k respectively) other top 8 customers. Loyalty programme, additional incentives, customer care etc. should be considered
- UK provides majority of revenue (84% across both years). Worthwhile continuing to invest promotional activities in this market, but may reach saturation point. YoY performance per country across a larger date range might reveal high growth countries. Countries 2-5 might be good to invest more time/resource in.
- Peak sales day varies a lot by month, however weekday sales consistently higher than weekend spend. Often a dip on Wednesday, so targetted ads and promos geared towards increasing spend on Tuesday & Thursday might help maximise revenues
- Peak sales hour fairly consistently around midday (presumably UK time). Considering low spend over the weekend, might suggest people are buying during their lunch break, either at work or at home. More segmented customer data would help ensure targeted ads and promotions reach the right people at the right time, capitalising on lunch break browsing and purchases.

## Improvements
- If this was an official project, I'd have allocated more time to separate out 2010 and 2011 data. The charts typically bucket all time data together, so YoY comparisons not really possible
- Plenty of product specific analysis missing, including product sales by month, distribution of purchase price, products by Customer ID etc.
- Growth-related metrics would be interesting to see. Countries sales growth, product sales growth
- I might be tempted to have dashboards on 2 or 3 tabs, one for each key area: Time Series metrics; Customer metrics; Product metrics
- If more ecommerce transactions were collected, I'm fairly confident the raw data and the analysis tabs (with all the Pivottables and calculations on) should be able to receive this and update automatically. The dashboard charts would likely need manually adjusting to reflect new data

## Caveats
- Original data set was fictious, but reasonably representative of a real-world set of ecommerce transaction records
- I stripped out all of the unallocated and non-standard records, to make the final data cleaner
- Two years of data was often grouped together, so the results displayed might be heavily skewed by annual differences
