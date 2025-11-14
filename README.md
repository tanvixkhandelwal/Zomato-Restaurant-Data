# **Zomato Restaurant Analytics Dashboard (Excel + Power Query + Power Pivot)**

A data-driven dashboard analyzing **8,600+ restaurants across Tier 1 & Tier 2 Indian cities**, uncovering trends in pricing, ratings, cuisine preferences and online delivery behavior using Excel, Power Query and Power Pivot.
>Interactive Excel dashboard comparing Tier 1 vs Tier 2 restaurant behaviour across cost, ratings, online delivery, cuisines, and table booking.

---

![Title Page](images/Zomato%20Restaurant%20All%20Cities%20Analysis.png)

---

## ** Features**
- **Excel + Power Query** for data cleaning, transformation, and automated refresh.  
- **Power Pivot (Data Model)** to build relationships and enable DAX measures.  
- **Interactive Dashboard** with slicers for Tier, Price Range, and KPI selections.  
- **Geographical Mapping** to visualize delivery penetration across cities.
- **Dynamic line chart** driven by dropdown selection (Ratings / Delivery / Table Booking / Cuisines).
- **Dynamic Line Charts** showing correlations between price range and behaviour (ratings, delivery, cuisines, table booking).  
- **Treemap Visuals & KPIs** for top cuisines, cost distribution, and city-level patterns.

---

## **Introduction**
Zomato is one of India’s largest food discovery and delivery platforms, hosting thousands of restaurants across multiple city tiers. The company gathers extensive data on restaurant characteristics such as pricing, ratings, cuisines, online delivery availability, and customer preferences.  
This project analyzes **Tier 1 vs Tier 2 restaurant behaviour** using Zomato’s aggregated dataset to understand affordability patterns, cuisine trends, delivery penetration, and customer satisfaction metrics.

---
## ** Business Objective**
The primary objective of this project is to analyze **restaurant behaviour across Tier 1 and Tier 2 Indian cities** to uncover differences in:
- Pricing patterns (budget, mid-range, premium, luxury)
- Online delivery adoption and geographical penetration
- Customer satisfaction trends (average ratings)
- Cuisine preferences and diversity across tiers
- Table booking behaviour and demand patterns

This dashboard helps identify:
- How affordability and customer expectations shift across city tiers  
- Which cuisines dominate in different markets  
- How delivery adoption varies by geography  
- Opportunities for expansion, marketing, and customer experience improvements  

---

## **Analytical Approach**

### **1. Data Preparation (Excel + Power Query)**
- Imported **Zomato’s multi-file JSON dataset** (40+ columns, ~30k records per file).  
- Used **Power Query** to clean and standardize data:
  - Removed duplicates and nulls  
  - Fixed data types and trimmed inconsistent text  
  - Filtered data to include **only Indian cities**  
  - Combined all files using **Append Queries**  
- Mapped cities into **Tier 1 / Tier 2** using a custom Excel mapping sheet.

### **2. Data Transformation (Excel + Power Pivot Basics)**
- Reduced dataset to **~8,600 usable restaurant records** for India.  
- Created additional columns using Excel formulas:
  - **VLOOKUP / XLOOKUP** → Tier classification  
  - **Nested IF formulas** → price range buckets & behavioural categories  
  - **ROUND(), CEILING(), UNIQUE(), SORT(), COUNTA(), OFFSET()** → dynamic behaviour  
- Built a lightweight **data model** (Power Pivot) only for structure — no DAX.  
- Ensured clean, analysis-ready fields for ratings, cuisines, booking, delivery, and price.

### **3. Dashboard Development (Excel)**
- Designed a fully interactive dashboard using only Excel formulas + visuals:  
  - KPI cards for average cost, rating, delivery %, booking %, top cuisine  
  - Treemap for cuisine distribution  
  - **Dynamic line chart** driven by data-validation dropdowns  
  - Tier-wise comparison visuals for cost, rating, delivery, and booking  
  - City-level online delivery penetration map  
  - Clustered column chart + thermometer chart for price segmentation

### **4. Insights & Quality Checks**
- Validated Tier-level KPIs using pivot tables.  
- Checked distribution accuracy for cuisines, price range, and ratings.  
- Ensured all dropdowns dynamically update all visuals correctly.

---
## ** Key Insights**

### **1. Tier-Level Restaurant Behaviour**
- **Tier 1 has 6,631 restaurants**, significantly more than Tier 2 (2,021), reflecting higher supply density in metros.  
- Despite higher competition, **Tier 1 restaurants charge slightly less** (₹620 avg cost for two) than Tier 2 (₹640), indicating stronger price competition.  
- **Tier 2 cities enjoy higher average ratings (4.01)** compared to Tier 1 (3.83), suggesting better customer satisfaction despite smaller markets.

### **2. Online Delivery & Booking Trends**
- **Online delivery availability:**  
  - Tier 1 → **29.08%**  
  - Tier 2 → **24.49%**  
  Tier 1 leads due to infrastructure, but Tier 2 still shows meaningful demand.
  
- **Table booking availability:**  
  - Tier 1 → **14.09%**  
  - Tier 2 → **8.76%**  
  Indicates that Tier 1 offers more premium dine-in experiences.

### **3. Cuisine Patterns**
- **Top cuisine:** *North Indian* in both tiers — strong pan-India preference.  
- Tier 1 shows **higher cuisine diversity**, while Tier 2 clusters around fewer dominant cuisines.  
- Cuisine concentration suggests opportunities for introducing niche cuisines in Tier 2.

### **4. Price-Behaviour Relationships**
- As **price range increases**, ratings generally rise but delivery availability drops.  
- **Higher-priced restaurants** focus more on dine-in; **lower-priced ones** dominate delivery.  
- The correlation patterns differ slightly between Tiers but follow the same broad trend.

### **5. City-Level Delivery Insights**
- Several Tier 1 cities show **strong delivery penetration**, aligning with urban demand and logistics networks.  
- Tier 2 cities show **promising but uneven delivery adoption**, suggesting potential for expansion in select markets.

---
## Dashboard Overview

### **Tier 1 Cities Dashboard**
![Tier 1 Dashboard](images/Zomato%20Restaurant%20Tier%201%20Cities%20Analysis.png)

### **Tier 2 Cities Dashboard**
![Tier 2 Dashboard](images/Zomato%20Restaurant%20Tier%202%20Cities%20Analysis.png)


## Dynamic Line Chart (Price Range vs Behaviour)

The line chart dynamically changes based on the selected behaviour metric.  
Below are screenshots of all four dropdown-driven variations.

### **1. Ratings vs Price Range**
![Dynamic Line Chart - Ratings](images/Zomato%20Restaurant%20Dynamic%20Line%20Chart%20Ratings.png)


### **2. Online Delivery % vs Price Range**
![Dynamic Line Chart - Delivery](images/Zomato%20Restaurant%20Dynamic%20Line%20Chart%20Delivery.png)


### **3. Table Booking % vs Price Range**
![Dynamic Line Chart - Booking](images/Zomato%20Restaurant%20Dynamic%20Line%20Chart%20Booking.png)


### **4. Number of Cuisines vs Price Range**
![Dynamic Line Chart - Cuisines](images/Zomato%20Restaurant%20Dynamic%20Line%20Chart%20Cuisines.png)


## ** Business Recommendations**

- **Expand delivery partnerships** in Tier 2 cities where demand is rising but supply is limited.  
- **Encourage premium restaurants** in Tier 1 to offer delivery for additional revenue streams.  
- Promote **diverse cuisines** in Tier 2 to tap into unmet customer interest.  
- **Reward programs or boosted visibility** for high-rated Tier 2 restaurants (4.01 average).  
- Use **price-behaviour correlations** to target customers with personalized offers based on cost brackets.  
- Improve table booking integrations in Tier 2 to attract premium diners.

---

## ** How to Use This Dashboard**

Since this project is shared through screenshots (not the Excel file), follow these steps to understand and navigate the analysis:
1. **Start with the Title Page**  
   View the overall project overview and the structure of the dashboard.
2. **Explore the All Cities Dashboard**  
   This view shows the full India-level restaurant landscape — KPIs, cuisine distribution, delivery penetration, and cost patterns.
3. **Compare Tier 1 and Tier 2 Dashboards**  
   Use the screenshots to understand how restaurant behaviour changes across:
   - Average cost for two  
   - Ratings  
   - Online delivery %  
   - Table booking %  
   - Cuisine diversity  
4. **Check the Dynamic Line Chart Screenshot**  
   The chart demonstrates how user-selected metrics (Ratings, Delivery, Cuisines, Table Booking) respond to different price ranges.
5. **Use the README insights section**  
   The key insights and recommendations summarize the findings so you don't need the actual Excel file.
6. **Refer to the Analytical Approach**  
   To understand how the transformations, mapping, tier classification, and formulas were applied using Excel + Power Query.

   ##  Contact  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/tanvikhandelwal30)  [![Email](https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail)](mailto:tanvikhandelwal14@gmail.com)  



![SQL Server](https://img.shields.io/badge/SQL%20Server-TSQL-blue?logo=microsoftsqlserver&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-DAX-yellow?logo=powerbi&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-Advanced-green?logo=microsoftexcel&logoColor=white)




