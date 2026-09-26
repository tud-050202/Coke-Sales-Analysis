Coca-Cola Sales Data Analysis

Project Overview

This project involves a comprehensive exploratory data analysis of beverage sales to identify key factors driving revenue. The analysis focuses on understanding seasonal trends, regional market performance, brand preferences, and retail partner contributions to optimize future sales strategies.

Data Source

File: Coke-sales-analysis-stubs_2.xlsx

Data Structure: Contains transactional sales data including Invoice Date, Region, Beverage Brand, Retailer, and Total Sales amounts.

Data Preparation & Cleaning

To ensure accurate aggregation in Excel, the raw data underwent the following preparation steps:

Header Formatting: Removed preliminary descriptive rows (Rows 1-3) to ensure standard column headers sit in Row 1.

Table Conversion: Converted the raw data range into a dynamic Excel Table (Ctrl+T) to allow for automatic updates when new data is added.

Date Extraction: Created a new calculated column named Month using the formula =TEXT([@[Invoice Date]], "mmmm") to enable seasonal and monthly trend analysis.

Key Analytical Dimensions

The analysis is driven by multiple Excel PivotTables, answering specific business questions:

1. Temporal Analysis (Sales by Month)

Goal: Identify the months with the lowest and highest sales.

Methodology: PivotTable grouping Total Sales by Month, sorted to reveal peaks (e.g., December, July) and troughs (e.g., March, September/October).

2. Geographic Performance (Sales Across Regions)

Goal: Determine which territories generate the highest revenue.

Methodology: PivotTable aggregating Total Sales by Region (West, Northeast, Southeast, South, Midwest), visualized using a standard Column chart.

3. Portfolio Performance (Sales by Brand)

Goal: Rank individual beverage brands by revenue generation.

Methodology: PivotTable aggregating Total Sales by Beverage Brand (Coca-Cola, Dasani Water, Diet Coke, Sprite, Powerade, Fanta), sorted from largest to smallest.

4. Partner Contribution (Sales by Retailer)

Goal: Assess the volume driven by specific retail partners.

Methodology: PivotTable aggregating Total Sales by Retailer (Sodapop, FizzySip, BevCo, DreamCo) to identify dominant distribution channels.

Cross-Variable & Matrix Analysis

To uncover deeper insights, the following multi-dimensional analyses were constructed:

Brand Seasonality (Brand vs. Month): A matrix PivotTable with Month in rows and Beverage Brand in columns, visualized via a Line Chart to track synchronized seasonal peaks and brand-specific dips throughout the year.

Regional Brand Preference (Brand vs. Region): A matrix PivotTable with Region in rows and Beverage Brand in columns, visualized via a Stacked Column Chart to compare overall territorial volume while highlighting the internal brand mix within each specific region.

Dashboard Interactivity

To make the analysis dynamic for end-users, Excel Slicers (for Region and Retailer) were inserted and report-connected to all respective PivotTables and PivotCharts. This allows stakeholders to instantly filter the entire dashboard to view, for example, how Brand Seasonality behaves strictly within the "West" region.
