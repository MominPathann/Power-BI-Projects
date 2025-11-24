# 📈 Financial Performance Analysis Dashboard: Awesome Chocolates

[✨ View Live Dashboard Here](https://app.powerbi.com/view?r=eyJrIjoiMjk1YTFmNjgtYzY5Ni00M2VlLWI4OTQtMjY1MWM1NTk2YmNlIiwidCI6ImRjNDliNmQyLTM1ZDQtNDM2Yi04Mzg4LWY1MThkOGRjYzNiZCJ9)

This Power BI dashboard was developed to enable executive leadership to track sales performance, operational efficiency, and key profitability metrics in near real-time. The solution uses advanced DAX measures for comparative analysis, transforming raw sales data into actionable business intelligence.

-----


### I. The Business Problem (Logic First)

Prior to this project, the "Awesome Chocolates" sales reporting relied on decentralized data sources, leading to a significant time lag and inconsistent metrics across regional teams. The lack of a unified view hindered proactive management intervention.

The objective was to evaluate the sales performance by tracking Key Performance Indicators (KPIs), including **Total Sales, Cost, and Profitability**, with the ultimate goal of identifying underperforming sales representatives and specific product lines to improve Month-over-Month (MoM) growth.

### II. Key Insights & Business Impact (The Result)

The consolidated dashboard immediately drove the following critical insights:

| Finding | Impact/Recommendation |
| :--- | :--- |
| **Revenue Risk:** While Year-to-Date (YTD) Total Sales stand at **$34M**, the company is experiencing a significant **10.6% Month-over-Month decline**, requiring immediate strategic adjustment. | **Action:** Prioritize analysis on high-volume, low-margin products identified on the Product Deep-Dive Tab to optimize pricing strategy and stabilize monthly sales. |
| **Profit Stability:** Despite the revenue drop, the company maintains a strong **60.35% profit margin**, indicating effective cost management ($13.52M Total Cost). | **Action:** Leadership is advised to focus intervention on sales and revenue generation, leveraging the high margin to support increased marketing spend. |
| **Sales Performance:** **Kelci Walkden** is the top performer in profit generation. However, lower-tier performers like **Ches Bonnell** are severely underperforming, highlighted by the red indicators in the salesperson matrix. | **Action:** Implement targeted coaching and training for the bottom 20% of the sales team, using the performance metrics available in the dashboard. |

### III. Technical Execution & Data Model (The Proof)

This project showcases end-to-end BI skills, including robust data modeling and advanced calculations:

  * **Data Model Architecture:** Implemented a Star Schema by linking 4 dimension tables (products, people, calendar, locations) to the central fact table (shipments), ensuring efficient query performance and relationship integrity. * Data Transformation (Power Query / M-Code): Used Power Query to unpivot regional sales columns into a single column (Sales), and merged the result with the geography dimension table to resolve a many-to-many relationship issue and simplify the fact table.
  * **DAX Measures Implementation:** *Implemented a [Rolling 90-Day Average Sales] measure using CALCULATE and DATESINPERIOD for trend smoothing, alongside critical MoM % Change measures for time intelligence reporting.*

### IV. Repository Contents

This repository is structured to provide full transparency of the project:

  * `/PowerBI_Source/`: Contains the final, anonymized **.pbix** file for full inspection of the data model and DAX code.
  * `/Data/`: Contains the anonymized raw data source file (e.g., raw-data.csv).
  * `/Screenshots/`: Contains high-resolution dashboard previews and GIFs.
![Portfolio-Dashboard](Portfolio-dashboard-screenshot(2).png)
![Portfolio-Dashboard](Portfolio-dashboard-screenshott.png)
