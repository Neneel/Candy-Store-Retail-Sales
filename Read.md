# Candy-Store-Retail-Sales
This repository contains detailed information about the Candy Store Retail Sales

# PROJECT TITLE: Candy Store Retail Sales

[Introduction](Introduction)

[Data Description](Data-Description)

[Methodology](Methodology)

[Visualizations](Visualizations)

[Findings](Findings)

[Recommendations](Recommendations)

## INTRODUCTION

Candy Distributors operates a broad and diverse distribution network, delivering a wide range of confectionery products across multiple regions and divisions. With operations supported by several factories and a portfolio of products spanning different categories, the company has significant potential for market growth and profitability. However, recent performance trends have revealed inconsistencies in sales outcomes across geographic areas and product lines, raising concerns about operational efficiency and goal alignment. 
Drawing from a unified dataset that includes sales transactions, product-level cost and pricing, factory geolocation data, and sales targets, this analysis aims to uncover actionable insights by:

•	Comparing actual sales against predefined targets for each division.

•	Identifying top-performing and underperforming products and regions.

•	Analyzing gross profit trends by product, factory, and region.

•	Exploring how factory locations align with regional demand patterns.

### Problem Statement

Despite having a broad distribution network and a diverse product portfolio, Candy Distributors faces inconsistencies in sales performance across regions and divisions. Current reporting methods offer limited insight into:

•	Which products are most and least profitable.

•	Division-wise progress toward annual sales targets.

•	How sales performance correlates with factory locations and regional demand.

This lack of visibility increases the risk of poor resource allocation, missed revenue opportunities, and operational inefficiencies. A centralized and interactive visual reporting solution is needed to empower management with the clarity required to take timely and informed action.

### Objectives
#### 1.	Identify Performance Gaps

Analyze sales and profitability data to pinpoint underperforming products, regions, and divisions that are not meeting expectations or contributing to business goals.

#### 2.	Measure Target Progress
Evaluate how actual sales compare against 2024 targets across different product divisions to monitor progress and highlight areas needing strategic focus.

#### 3.	Optimize Product and Factory Performance
Assess product profitability and factory efficiency to identify opportunities for cost reduction, pricing strategy improvements, and supply chain optimization.

#### 4.	Enable Data-Driven Decision-Making
Deliver clear, visual insights through an interactive Power BI dashboard that equips management with the tools to make timely, informed business decisions.


## DATA DESCRIPTION
The dataset comprises four main tables: Sales, Factories, Products, and Targets, each contributing essential data for analyzing business operations, production, and performance tracking.

#### 1.	Sales Table
This table captures all customer orders and transaction-level details. It includes:

Row ID: Unique row identifier

Order ID: Unique order identifier

Order Date: Date of order

Ship Date: Date of shipment

Ship Mode: Shipping method of the order

Customer ID: Unique customer identifier

Country/Region: Country or region of the customer

City: City of the customer

State/Province: State or province of the customer

Postal Code: Postal code / ZIP code of the customer

Division: Product division 

Region: Region of the customer

Product ID: Unique identifier for the product

Product Name: Long name of the product

Sales: Total sales value of the order

Units: Total number of units ordered

Gross Profit: Gross profit of the order (calculated as Sales – Cost

Cost: Manufacturing cost of the order

#### 2.	Factories Table
This table provides location details for each factory involved in manufacturing.

Factory: Factory Name

Latitude: Latitude Coordinates

Longitude: Longitude Coordinates

Division: Product Division

#### 3.	Products Table
This table outlines detailed product specifications and associations with factories.

Product Name: Product Descriptive Name

Factory:  Factory Name

Product ID: Product Unique Identifier

Unit Price: Selling Price of Product

Unit Cost: Cost to Produce Product

#### 4.	Targets Table
This table stores predefined sales targets segmented by product division for the year 2024.

Division: Product Division

Target: Sales Target 2024

## METHODOLOGY
To achieve the analysis objectives, a structured and data-driven approach was adopted, integrating multiple data sources and leveraging PowerBI features. The methodology involved the following key steps:

### 1. Data Collection and Integration

•	Consolidated data from four primary tables: Sales, Products, Factories, and Targets.

•	Ensured data consistency by joining tables using common fields such as Product ID, Division, and Factory Name.

•	Verified data quality by checking for missing values, duplicates, and inconsistencies in date formats, geographic data, and financial figures.

### 2. Data Cleaning and Transformation

•	Standardized column formats (e.g., dates, currency, region names).

•	Calculated derived fields, including: 

Gross Profit = Sales − Cost

Profit Margin = (Gross Profit / Sales) × 100

Target Achievement % = (Actual Sales / Target) × 100

### 3. Exploratory Data Analysis (EDA)

•	Conducted trend analysis on sales and gross profit across time, products, and regions.

•	Used descriptive statistics and visual summaries to identify:

i.	High and low-performing products.

ii.	Underperforming regions and divisions.

iii.	Sales patterns relative to factory locations and customer distribution.

### 4. Dashboard Development in Power BI

Designed an interactive Power BI dashboard with filters and drill-down features for:

•	Sales vs. Target by Division

•	Product-Level and Factory-Level Profitability

•	Regional Sales Distribution and Factory Mapping

•	Incorporated KPI indicators, bar charts, maps, and slicers to enhance user interaction and insight discovery.

## VISUALIZATONS
<img width="505" alt="Screenshot 2025-05-11 180703" src="https://github.com/user-attachments/assets/d7a09767-efca-4d5a-95d6-f35aebabc529" />
<img width="505" alt="Screenshot 2025-05-11 180757" src="https://github.com/user-attachments/assets/99f83013-b89b-4c1d-99cb-16719b3c22b2" />
<img width="506" alt="Screenshot 2025-05-11 180904" src="https://github.com/user-attachments/assets/d07bd15e-a214-4927-9c2d-31c6a6806e27" />

### MODELLING
<img width="757" alt="Screenshot 2025-05-11 181253" src="https://github.com/user-attachments/assets/12f45ee0-2f22-442b-a425-ea9136fd912f" />

## FINDINGS
### 1.	Identify Performance Gaps

#### a.	Underperformance in Sugar Division:

•	Only $144 in 2024 sales vs. Year 2024 $15,000 target.

•	Despite a high margin (65.05%), volume is critically low.

#### b.	Uneven Product Contribution:

•	Chocolate contributes 95.06% of total profit, shows dependency on one product line.

•	Products like Fun Dip, Nerds, Sweet TARTS, and Laffy Taffy are contributing little to revenue or profit.

#### c.	Factory Disparity:

•	Lot’s O’ Nuts and Wicked Choccy’s dominate sales.

•	Factories like Sugar Shack, The Other Factory, and Secret Factory have negligible performance.

### 2.	Measure Target Progress

#### a.	Chocolate Division:

•	Exceeded target massively: $43.38K in sales vs. $27K target

#### b.	Other Division:

• Moderate performance: $3.44K in sales vs. $3K target

#### c.	Sugar Division:

• Severe shortfall: $144 in sales vs. $15K target

#### d.	2024 Sales Target Achievement:

• 2024 Sales target achievement rate is 104.37%, suggesting effective resource allocation.

#### e.	Profit Margin:

• Overall profit margin is strong at 65.91%, aligning well with profitability goals

### 3.	Optimize Product and Factory Performance

#### a.	Top Products to Leverage:

•	Wonka Bar – Triple, Fudge, Original: High sales and high profit

•	Everlasting Gobstopper, Hair Toffee: Excellent profit margins (>80%)

#### b.	Low-Yield Products to Review:

•	Fun Dip, Nerds, Katookles, Wonka Gum: Low sales and/or profit

#### c.	Factory Optimization:

•	Lot's O' Nuts leads in both volume (51.28K units) and sales ($76.34K)

•	Wicked Choccy’s also performs well ($55.35K)

•	Low-output factories like Secret Factory, Sugar Shack need investigation

#### d.	Cost Efficiency:

•	Average unit cost is low at $1.81, allowing healthy margins

### 4.	Enable Data-Driven Decision-Making

#### a.	Geographic and Factory-Level Insights:

The dashboards provide clear visibility into where sales are originating, with the United States being the dominant contributor. This enables leadership to assess potential in underperforming regions, such as Canada, and make informed expansion or investment decisions.

#### b.	Product-Level Performance Metrics:

Detailed data on each product’s sales, costs, and profit margins allow the team to evaluate which items drive profitability. This insight supports strategic decisions around inventory, marketing focus, and product development.

#### c.	Division Profitability Analysis:

The Chocolate division is responsible for the majority of profit generation. With division-level metrics, the organization can assess where to allocate more resources and which areas require corrective action.

#### d.	Sales and Profit Trends Over Time:

Historical performance visuals show consistent growth in both sales and profit. These trends can inform forecasting, budgeting, and long-term planning.

#### e.	Pricing Strategy Optimization:
With an average unit cost of $1.81 and an average selling price of $4.46, there is strong margin potential. This data can guide pricing strategies, particularly for high-performing products.

## RECOMMENDATIONS
### 1.	Revamp the Sugar Division Strategy

•	Investigate root causes of severe underperformance despite strong profit margins.

•	Reassess product positioning, marketing, and distribution efforts.

### 2.	Diversify Revenue Sources

•	Reduce dependency on the Chocolate division by boosting visibility and investment in underperforming yet potential-rich products like Nerds and Laffy Taffy.

•	Conduct A/B testing on promotional offers for low-yield products.

### 3.	Rationalize and Optimize Factories

•	Consider scaling operations at Lot’s O’ Nuts and Wicked Choccy’s.

•	Audit underperforming factories (e.g., Sugar Shack, Secret Factory) for operational inefficiencies or resource misalignment.

### 4.	Leverage High-Profit Products

•	Prioritize products like Everlasting Gobstopper and Hair Toffee with high margins for promotional focus and wider distribution.

•	Bundle high-performing SKUs with low performers to increase basket value.

### 5.	Enhance Geographic Penetration

•	Explore untapped regions like Canada with tailored go-to-market strategies.

•	Use location-based performance data to guide salesforce deployment and regional campaigns.

### 6.	Data-Driven Pricing & Forecasting

•	Maintain or improve pricing strategy given healthy margins (65.91%).

•	Use profit and sales trends to improve demand forecasting and set realistic division-level targets.

### 7.	Refine Sales Targets and KPIs

•	Set more balanced and realistic targets per division to reflect past performance and market potential.

•	Continue tracking target achievement rates across divisions to drive accountability.

