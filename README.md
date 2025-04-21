**Superstore EDA Project using Seaborn**


**Overview:**

This project performs an Exploratory Data Analysis (EDA) on the Superstore dataset using Python. The analysis includes data cleaning, basic exploration, statistical analysis, and visualizations to uncover insights about sales, profits, and customer behavior across regions, categories, and shipping modes.
Dataset


**The dataset (superstore.csv) contains 9,994 rows and 21 columns, detailing sales transactions with attributes such as:**

Order Details: Order ID, Order Date, Ship Date, Ship Mode

Customer Information: Customer ID, Name, Segment

Geographical Data: Country, City, State, Postal Code, Region

Product Information: Product ID, Category, Sub-Category, Product Name

Financial Metrics: Sales, Quantity, Discount, Profit



**Project Structure:**

EDA_Superstore.pdf: Documentation of the EDA process, including code snippets and visualizations.

superstore.csv: The raw dataset used for analysis.

cleaned_store.csv: Cleaned dataset after preprocessing.

sample_pivot.csv: Pivot table output summarizing sales by region and category.

scripts/: Python scripts for data analysis and visualization.

visualizations/: Generated plots (e.g., histograms, bar plots, heatmaps).



**Requirements**

To run the analysis, install the following Python libraries:

pip install pandas numpy matplotlib seaborn



**Analysis Steps**


**Data Loading and Cleaning:**

Loaded the dataset using pandas.

Standardized column names (lowercase, replaced spaces with underscores).

Converted order_date and ship_date to datetime format.

Checked for missing values (none found) and duplicates (none found).



**Basic Exploration:**

Dataset shape: (9994, 21).

Column data types: Mix of int64, float64, and object.

Summary statistics and unique value counts for categorical columns.



**Data Analysis:**

Total Sales by Region: West ($725,457.82), East ($678,781.24), Central ($501,239.89), South ($391,721.91).

Average Sales by Category: Technology ($452.71), Furniture ($349.83), Office Supplies ($119.32).

Sales by Ship Mode: Standard Class ($1.36M), Second Class ($459,193.60), First Class ($351,428.40), Same Day ($128,363.10).

Monthly Trends: Aggregated sales and profit by month.

Filtering: Identified high-value sales (> $1000) and regional subsets.



**Visualizations:**

Distribution Plot: Sales distribution (< $1000) by category.

Joint Plot: Sales vs. Profit, colored by category.

Pair Plot: Relationships between numerical variables, segmented by region.

Bar Plot: Sales by category and region.

Count Plot: Category counts by region.

Box Plot: Profit distribution by category.

Scatter Plot: Sales vs. Profit, colored by category.

Correlation Matrix: Heatmap of correlations between sales, profit, quantity, and discount.



**Data Export:**

Saved cleaned dataset as cleaned_store.csv.

Exported pivot table (sales by region and category) as sample_pivot.csv.



**Key Insights**

Regional Performance: The West region leads in total sales, while the South has the lowest.

Category Trends: Technology products have the highest average sales, followed by Furniture and Office Supplies.

Profit Variability: High sales do not always correlate with high profits due to discounts (e.g., negative profits in some high-sales transactions).

Shipping Impact: Standard Class shipping dominates in sales volume.

Correlation: Weak correlation between sales and profit (visualized in heatmap).



**Future Improvements**

Add time-series analysis to explore seasonal trends.

Incorporate customer segmentation for targeted marketing insights.

Implement interactive dashboards using Plotly or Dash.

Analyze discount impact on profitability in greater detail.



**License**

This project is licensed under the MIT License. See the LICENSE file for details.



**Contact**

For questions or feedback, please contact singhpravesh882@gmail.com.
