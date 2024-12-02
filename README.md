## Project Overview
This project centers on analyzing sales data for a beverage industry, with each step guided by specific business requirements and questions to uncover valuable insights into product performance and customer demographics.

## Business questions
The image below provides a snapshot of the business questions that guided the analytical process throughout this project.

![Screenshot 2024-11-27 063005](https://github.com/user-attachments/assets/8dcdd3dc-8ce3-4358-835c-9225ea5c493f)

To optimize its operations and enhance customer service, the business enlisted the expertise of a data analyst to analyze its data and uncover actionable insights based on key questions.

As the consultant, the following steps were taken to address the business questions:

**Data Importation/Cleaning and Manipulation:**

I downloaded the dataset and imported it into Excel Power Query for data cleaning and manipulation.

The dataset consisted of multiple tables, including:
- A fact table containing 20,000 rows and 7 columns
- Dimension tables, such as Salesperson, Store Target, Customer, and Product tables, which were linked to the fact table during the data modeling process.

To generate trend-based insights, as required by the business questions, I created a Date Table derived from the Order Date. This was crucial for analyzing temporal patterns effectively.

Additionally, I created a separate table to store all measures for better organization.

After completing the data cleaning process, I loaded the data into the Data Model rather than the workbook. This approach allowed seamless data modeling. Following this, I switched back to the Excel workbook to begin the analysis, as the project was conducted entirely in Microsoft Excel.

![Screenshot (100)](https://github.com/user-attachments/assets/b8d1ae06-c98e-40ad-83ca-e6eab3330964)


To address business questions related to metrics like revenue and profit, I utilized the **SUMX** function. This was necessary because the data structure revealed that the **Order Quantity** column was in the Fact table, while the **Cost Price** and **Selling Price** columns were in the Product table. By leveraging SUMX, I was able to calculate these metrics dynamically across the related tables in the data model. 

![Screenshot (102)](https://github.com/user-attachments/assets/f888233b-2549-42b8-b31d-84fbcd8aecae)
![Screenshot (101)](https://github.com/user-attachments/assets/2adbb5b9-1ff8-441d-9cc5-891e2d292802)


To perform an in-depth analysis of the business questions, I created the following measures:

![Screenshot 2024-11-27 073800](https://github.com/user-attachments/assets/416465c4-a0b5-4c95-9a96-739163e5f635)


The business questions covered various aspects of the company’s operations over the years, making it impractical to display all insights in a single dashboard. To address this, I segmented the questions into distinct categories, resulting in three focused dashboards: the Store Dashboard, the Profit Over Time Dashboard, and the Product-Customer Dashboard. This segmentation ensures easier navigation and allows the business to explore key areas efficiently.

## Key insights from the Store Dashboard

![Screenshot (92)](https://github.com/user-attachments/assets/c1ffaf3a-f058-45f1-b429-90b42f46da73)

This dashboard highlights store performance, showcasing insights on stores that met their targets and those that did not. Key KPIs were derived from the measures created earlier, excluding the variance. To calculate variance, I subtracted the target from revenue and divided the result by the target.

To effectively compare target versus revenue for each store and identify high-performing and underperforming locations, I leveraged the Microsoft Add-Ins feature, specifically selecting the **Zebra BI Tables for Office** tool to enhance the visualization and analysis.

![Screenshot (104)](https://github.com/user-attachments/assets/7186d9fa-25a8-4003-8160-4c5bf3c7f235)

This method is ideal for comparison, as it automatically generates detailed insights about the items being analyzed.

Focusing on store performance, the dashboard clearly identifies all stores that exceeded their targets and those that fell short, providing a clear overview of successes and areas needing improvement.

For instance,Lee-Myers ($548.4K, 31.1% above target), Myers-Lopez ($565.2K, 26.7% above target), e.t.c, achieved positive variances from their targets. While stores like Novak PLC ($536.2K, 24.6% below target),Miller ($547.5K, 15.3% below target), e.t.c struggled to meet their targets.

Generally, Total revenue of $5.4M surpassed the target of $5.3M, showing a positive variance of 3.7%


## Key insights from the Timeframe Dashboard
![Screenshot (93)](https://github.com/user-attachments/assets/74a87eec-fd86-439e-aa01-62256137dcb5)


**1. Quaterly Performance:**

Q1 and Q2 showed growth of +3.6%, while Q3 (-1.6%) and Q4 (-0.0%) saw a slowdown.

**2. Revenue by weekday and weekend:**

Weekdays contributed 71% of revenue, averaging $4M. Weekends generated 29% of revenue ($2M).

**3. Monthly performance:**

Strong months included August (+12.5%), October (+10.8%), and November (+11.9%).

Revenue dipped in July (-5.0%) and December (-3.4%).


## Key insights from the Profit view Dashboard
![Screenshot (94)](https://github.com/user-attachments/assets/0f6e271a-d2fd-440e-8eae-061c9ce74362)


**Profit Margin:**

Profit margin Achieved an impressive 42.18% margin with $2.3M total profit.

**Customer demographics:**

- Male customers contributed 51.47% of profits, while female customers accounted for 48.53%.

- The 51+ age group generated the highest profit ($921K), followed by the 41–50 age group ($483K).


**Most profitable products:**

- Begin Brew led profitability with $95K, followed by Common Splash ($85K) and Onto Dew ($83K).

- Soft drinks drove the most Profit ($718K), significantly outperforming other categories like sports drinks ($417K).



Based on the dashboards and data shared, here’s how the analysis could inform real-world business decisions in the same industry:

**1. Resource Allocation**

- *Top-Selling Product Categories:* 
  
  If certain product categories (e.g., soft drinks or alcoholic beverages) consistently outperform others, the company can allocate more shelf space, inventory, and marketing budget to these items.

- *Regional Performance:*
  
   Insights into regional sales trends help determine where to focus distribution and staffing efforts. For example, if a specific region has high sales of sports drinks, resources can be allocated to increase stock or promotional campaigns there.

- *Low-Performing Products:*
  
   For products with low sales, the business can evaluate whether to reduce inventory, rebrand, or discontinue them, freeing up resources for high-demand items.


**2. Customer Targeting**

- *Demographic Preferences:*

  If the dashboards provide insights into customer preferences (e.g., age group or income level favoring certain beverages), the company can tailor advertising and promotions to these segments.

- *Seasonal Trends:*
  
   Sales spikes for specific products during certain months (e.g., soft drinks in summer) can guide targeted seasonal campaigns.


- *Promotional Strategies:*

   If discounts or bundles drive sales in a particular category, these strategies can be refined and targeted toward customers who prefer those items.



**3. Inventory Management**

- *Demand Forecasting:* 
  
  By analyzing trends, the company can predict demand for each product category, ensuring adequate stock and reducing waste or overstocking.

- *Supply Chain Optimization:*
  
   Knowing which products are most popular in specific regions allows for optimized delivery routes and minimized stockouts.



**4. Marketing Strategy**

- *Product-Specific Campaigns:* 

  Insights into the best-performing and fastest-growing product categories help design targeted campaigns, such as promoting energy drinks to sports enthusiasts.
