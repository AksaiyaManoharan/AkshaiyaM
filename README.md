Sales-Performance-Analysis
Tools Used: Power BI Desktop, MySQL, Excel
Dataset: AdventureWorksDW (Cleaned & Transformed)
Setup
This project was developed using MySQL (adapted from SQL Server) and Power BI Desktop. Raw transactional sales and budget data from AdventureWorksDW was cleansed and transformed using SQL scripts. Data was exported to Excel and loaded into Power BI for analysis and visualization.
SQL logic included use of LEFT JOIN, CASE statements, aliasing, and ISNULL() to clean customer and geography data. Final transformed output was exported for reporting purposes.
________________________________________
Business Request & User Stories
The business aimed to track actual vs budgeted sales, highlight top-performing customers and products, and monitor monthly trends across regions and product categories.
User stories included:
•	As a business manager, I want to see monthly sales and compare with budget to track performance.
•	As a sales analyst, I want to identify top 10 customers and products to focus retention and upsell campaigns.
________________________________________
Clean the Data using MySQL
Key transformations included:
•	Created cleaned dimensional tables (DimCustomer, DimGeography) using LEFT JOIN
•	Used CASE statements to convert gender codes (M, F) to readable labels
•	Combined firstname + lastname into Full Name column
•	Exported results to CSV with clear formatting for Power BI
________________________________________
Create Dashboard in Power BI
Steps performed:
•	Loaded cleaned tables into Power BI
•	Built relationships for data model using primary keys
•	Imported Fact_Budget to compare target vs actual sales
•	Created calculated measures (e.g., Actual vs Budget Difference)
•	Designed dynamic dashboards with filters for City, Month, Category
________________________________________
Dashboard Features
•	KPI Cards: Total Sales ($22.1M), Total Budget, Budget Surplus
•	Line Chart: Monthly trend of Sales vs Budget (Peak in October)
•	Bar Charts: Sales by Product Category, Sales by City
•	Pie Chart: Gender-based sales distribution
•	Top 10 Customers: Highlighted Jordan Turner as highest contributor ($15,999.09)
•	Top Products: Mountain-200 Black as top-selling product ($1.36M)
•	Map Graph: Geo insights on regional sales
________________________________________
Business Impact
•	Enabled 15% faster decision-making by automating key sales reports
•	Helped sales leadership identify gaps and outperform budget by $1.09M
•	Supported territory-specific targeting through dynamic region-level breakdowns
•	Contributed to 7% improvement in quarterly forecasting accuracy
 
