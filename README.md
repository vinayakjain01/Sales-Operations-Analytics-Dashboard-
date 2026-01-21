# Sales Operations Analytics Dashboard 📊
📌 Project Overview
Role: Data Analyst Intern | Company: Madvertise Timeline: July 2024 – Sept. 2024

This project involves an end-to-end analysis of sales and logistics data for an e-commerce operation. The goal was to transform messy operational data into a clean, actionable Power BI dashboard to track revenue, delivery efficiency, and customer retention.

The final dashboard analyzed 100,000+ records, tracking ₹53.91M in revenue and providing visibility into the delivery supply chain.

💼 Business Problem
The stakeholders faced challenges in tracking order fulfillment and identifying revenue leakage caused by high Return to Origin (RTO) rates. The raw data was scattered across disparate files with inconsistent formatting, making it difficult to answer key questions:

Which regions are driving the most sales?

Why is the delivery success rate hovering at ~71%?

What is the ratio of New vs. Returning customers?

🛠️ The Solution
I built a 3-page interactive Power BI dashboard that serves as a central source of truth for sales and operations teams.

Key Features:
Executive View: High-level KPIs (Revenue, AOV, Total Orders) and geographic sales distribution.

Logistics & Efficiency: Deep dive into RTO % (Return to Origin), courier performance, and delivery success rates.

Customer Intelligence: Analysis of retention trends (New vs. Returning) and top-performing customer segments.

🔍 Key Insights & Discovery
Analysis derived from the dashboard data:


Revenue Concentration: A significant 51.69% of total sales comes from a single state (Punjab), with the top 5 cities (Amritsar, Jalandhar, Patiala, etc.) driving the bulk of revenue.



Logistics Bottlenecks:

The overall Delivery Success Rate is 71.45%, with a concerning RTO (Return to Origin) rate of 28.46%.


State-level drill-downs revealed extremely high RTO rates in specific regions like Arunachal Pradesh (53.33%) and Tripura (46.67%), signaling a need for courier partner re-evaluation in the North East.


Payment Risk: There is a massive reliance on Cash on Delivery (COD), comprising ~99% of orders (93.4K COD vs. 1K Prepaid). This correlates strongly with the high RTO rate, as COD orders are more likely to be rejected at the doorstep.


Customer Retention: The business showed a positive trend in customer loyalty. Sales from returning customers grew from ~50% in January to ~69% by December, indicating strong product satisfaction despite logistics challenges.



<img width="1274" height="723" alt="image" src="https://github.com/user-attachments/assets/98142632-9a72-441b-bf8a-409b064ed063" />
<img width="1278" height="730" alt="image" src="https://github.com/user-attachments/assets/40d70ca3-c0b3-4742-a84f-3351d1499111" />



⚙️ Technical Process
1. Data Cleaning & Transformation (ETL)
Source: Raw Excel/CSV files containing 100,000+ rows of order data.

Standardization: Used Power Query to normalize city names (e.g., correcting spelling errors in "Jalandhar", "Ludhiana").

Modeling: Established a Star Schema connecting Fact tables (Orders) with Dimension tables (Customers, Locations, Products).

2. Metric Calculation (DAX)
Implemented complex DAX measures to calculate custom KPIs:

Delivery % = DIVIDE([Delivered Orders], [Total Orders])

RTO % = DIVIDE([Returned Orders], [Total Orders])

New vs Returning segmentation logic based on customer order history.

3. Visualization
Used Decomposition Trees to analyze root causes of high RTO.

Implemented Ribbon Charts to track the shift in New vs. Returning customers over time.

Designed Geospatial Maps to visualize state-wise penetration.

🚀 How to Run
Clone the repository:

Bash

git clone https://github.com/yourusername/Sales-Operations-Dashboard.git
Open the .pbix file in Microsoft Power BI Desktop.

The data source is currently linked to the static Excel file included in the data folder. You may need to update the data source path via Transform Data -> Data Source Settings.

📬 Contact
Your Name [LinkedIn Profile Link] | [Email Address
