# Sales, Profit, and Returns Analysis Report
Author: sreejitha

Date: 28/11/2024

# Overview
This project analyzes sales, profit, and return trends for a global store. The report is designed to provide stakeholders with actionable insights into the store’s performance across countries, regions, and markets.

The analysis includes:

* Total Sales, 
* Total Profit,
* profit margin
* Average Shipping Costs 
* total customer
* top sold category
* total quantity
* total Returns
* return rate as KPIs.

Sales and profit trends by region, market, and product category.
Analysis of returned sales and return rates.
Interactive visualizations and drill-down capabilities.

#### Source Data:

Imported data from an Excel file with multiple sheets (Orders, Returns, etc.).

#### Data Cleaning:

   Removed duplicates and null values.
Standardized date formats and region names for consistency.
Ensured relationships between the Orders and Returns tables using the Order ID field.
#### DAX Measures:

Created new measures for advanced calculations:
Total Sales: SUM(Orders[Sales])
Total Profit: SUM(Orders[Profit])
Average Shipping Cost: AVERAGE(Orders[Shipping Cost])
Returned Sales: Sales tied to returned orders using DAX filters.
Return Rate: Ratio of returned orders to total orders.

#### Visualizations

* Map Visualization
 ##### Purpose: 
To display sales geographically by country,region, and market.
Key Insights: Countries or cities with high sales volumes and their respective profit margins.
Fields:
Location: Country/market,region
Values: Sales, Profit

* KPI Cards
##### Purpose:
``` To highlight key metrics at a glance.

Metrics:

Total Sales: Displays overall sales performance.
Total Profit: Tracks overall profitability.
Average Shipping Cost: Monitors cost efficiency.
Visual: Single-value cards with clear formatting (currency and percentage).
```
* Stacked Bar Chart
Visualization: Returned Sales vs. Total Sales by Region
##### Purpose:

 ```To identify regions with the highest proportion of returned sales.
Fields:
Axis: Region
Values: Total Sales, Returned Sales
Key Insights:
Regions with high return rates (potential product or customer service issues).
Visual comparison of total and returned sales for better decision-making.
```
* Matrix Table
##### Purpose: 

```To provide drill-down functionality for hierarchical data analysis.
Fields:
Rows: Market > Region > State > City
Values: Sales, Profit
Capabilities:
Interactive drill-down to explore sales and returns at a granular level.
Conditional formatting to highlight outliers.
```

* Shipping Percentage by Ship Mode (Pie Chart)

##### Purpose: 

```Helps in identifying popular shipping methods and analyzing cost-effectiveness.```

* Shipping Cost by Ship Mode (Donut Chart)

##### Purpose:
 ```Analyzes the cost associated with each shipping mode to determine cost-efficiency.Shows the total shipping cost distribution across different ship modes.```

* Dynamic Slicers:
``` 
    1. By Region,
    2. market
    3. segments
    4. Year
    5. ship mode

```

##### Drill-Down Capabilities:


Navigate from market to market,country,region, state, and city in the matrix and charts.
Conditional Formatting:
Highlights profitable and non-profitable areas for better focus.

# How to Use the Report
### Explore KPIs:

Review the top-level metrics to understand overall performance.
Analyze by Region:
Use the map and stacked bar chart to identify regions driving sales and profit.
### Identify Trends:
Use the matrix table and maps to detect patterns in returns and sales.

### Focus on Improvements:
Look for regions, products, or customer segments with high return rates to implement targeted improvements.

# Conclusion
This report integrates sales, profit, and returns data to provide a holistic view of the store's performance. The insights help stakeholders identify growth opportunities, manage costs, and address return-related issues effectively.






