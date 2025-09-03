README - KPI Sales Performance Dashboard Project

Author: Fernando Del Valle | Psycollapse @ 2025

Project Overview

This project demonstrates a Tableau dashboard built from a synthetic dataset that simulates marketing and sales performance. The goal is to showcase KPI tracking, ROI analysis, and interactive drilldowns that mirror a real-world BI analyst workflow. It is designed as a portfolio piece to demonstrate data preparation, dashboard design, and storytelling for stakeholders.

Folder Structure

tableau/

└── kpi\_db\_salesPerformance-01/

├── data/

│ ├── marketing\_sales\_raw.csv (original dataset)

│ └── marketing\_sales\_reconciled.csv (processed dataset with calculated fields)

├── workbook/

│ └── kpi\_salesPerformance.twbx (Tableau packaged workbook)

└── README.txt (this file)

└── KPI\_dashboard\_01.pdf

Dataset Details

*   marketing\_sales\_raw.csv: Synthetic dataset with ~500 rows. Fields include date, channel, campaign, region, sales\_rep, spend, impressions, clicks, conversions, revenue.
    
*   marketing\_sales\_reconciled.csv: Processed dataset exported from Tableau, includes additional calculated measures used in the dashboard such as CTR, CPC, Conversion Rate, ROAS, and Avg Deal Size.
    

Key KPIs

*   CTR (Click-Through Rate) = clicks /
    
*   CPC (Cost per Click) = spend /
    
*   Conversion Rate = conversions /
    
*   ROAS (Return on Ad Spend) = revenue /
    
*   Avg Deal Size = revenue /
    

Dashboard Features

*   KPI cards: Spend, Revenue, Conversions, ROI/
    
*   Trend analysis: Revenue and Spend over
    
*   Channel performance: ROAS vs CPC
    
*   Sales rep performance: Revenue and conversions by
    
*   Campaign drilldown: Scatter plot showing ROI vs CPC by
    
*   Filters: Channel, Region, Date
    
*   Interactivity: Filters applied across all views, parameter toggle to switch KPIs
    

Usage Instructions

*   Open the .twbx file in Tableau Public
    
*   Connect to the dataset in the data folder if needed (CSV
    
*   Explore the dashboard interactively by applying filters and reviewing
    
*   For a live view, publish the workbook to Tableau Public and share the
    

Purpose

*   This project is intended as a demonstration of BI reporting and dashboarding skills. It highlights the ability to prepare raw data, reconcile it into a clean reporting source, and build an executive-style Tableau dashboard that delivers actionable insights. It can be reused as a template for similar marketing and sales analysis projects.