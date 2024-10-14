# Real-Estate-Market-Data-Analysis
Data analysis and visualization of real estate sales

Overview:
This project focuses on analyzing and visualizing real estate sales data, including customer demographics, building preferences, and sales trends across years. It highlights how macroeconomic events, such as the 2008 financial crisis, influenced the sales volume and buyer behaviors. The insights gathered can support real estate developers and marketers in optimizing sales strategies and customer targeting.

Table of Contents:
Introduction
Data Source
Insights
Visualizations
Conclusion
Requirements
How to Use

Introduction:
This analysis focuses on profiling customers, understanding property trends, and identifying key time periods for sales in real estate. It leverages sales data to create customer personas, identifies building types with the highest deal satisfaction, and provides recommendations on future strategies for targeting specific customer groups and building types.

Datasets:
The data used in this analysis contains records of property sales, customer demographics, property characteristics, and geographic data. Preprocessing was conducted to clean and format the data before generating the key insights.

## Datasets

The following datasets are included in this repository:

- `customers.csv`: Contains customer information such as customer ID, birth_date, country, deal satisfaction, mortgage, and purchase details.
- `properties.csv`: Contains information about the properties sold, including property ID, type, price, area, status, and sale date.

Usage

These datasets are used for analysis in the project. You can load them using `pandas`:

#python
import pandas as pd

# Load the datasets
customers = pd.read_csv('customers.csv')
properties = pd.read_csv('properties.csv')

Insights:
1. Customer Profile:
The age at which most customers purchase a home is between 31 to 42.
Most properties are purchased by financially stable individuals around their mid-30s to early 40s.
This demographic can be targeted through platforms such as Facebook, YouTube, and Google Ads for future marketing campaigns.

2. Building Characteristics:
Building types 2 and 3 have the highest total sales, while Building type 4 leads in both average price and deal satisfaction.
Type 4 buildings tend to be more luxurious and spacious, which justifies their higher price. These are not sold as frequently but provide higher customer satisfaction.
Customers are more likely to buy smaller and less expensive building types, as indicated by the trends in our dataset.Real estate developers can consider this information when devising their strategies.
Real Estate developers may consider investing in more luxurious properties for high-end customers that would create a higher deal satisfaction or focus on standard types (types 2 and 3) for more frequent sales.

3. Sales by Country:
The majority (90%) of sales come from the United States, indicating a highly localized market. International sales are significantly lower, with countries like Canada, Belgium, and Russia contributing minimally.

4. Sales Trends Over Time:
2007 was the peak year for sales, with a notable drop-off in subsequent years, particularly in 2009, likely due to the global financial crisis.
Understanding this sales pattern can help developers strategize for market downturns and adjust sales approaches accordingly.

Visualizations:
Key visualizations included in this project are:

Stacked Area Chart: Displaying yearly sales distribution across buildings (total_sales_per_year_per_building_stacked_area_chart_v2.png)
Line Chart: Depicting the total revenue generated from 2004 to 2010 (total_revenue_per_year_in_M_line_chart.png)
Pareto Chart: Segmenting customers by state in terms of frequency of purchases and cumulative distribution (US_segmentation_by_state_pareto_diagram.png)
Each chart provides a unique perspective on the data, offering a more intuitive understanding of sales distribution and customer behavior.

Conclusion:
This analysis offers valuable insights into customer demographics, property characteristics, and sales trends. It highlights the importance of targeting specific age groups for marketing efforts, choosing the right mix of property types for development, and understanding the impact of macroeconomic events on sales patterns. These insights can guide real estate developers and marketers in targeting potential buyers and optimizing sales strategies.

Next Steps
Future analysis can focus on:

Expanding the dataset to include more recent sales data.
Analyzing specific customer feedback to improve deal satisfaction.
Evaluating other market factors, such as interest rates and their correlation with sales volumes.

Requirements:
Python 3.x
Pandas
NumPy
Matplotlib
Seaborn

