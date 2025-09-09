Author: Fernando Del Valle | Psycollapse @ 2025

Project Overview

This project demonstrates a Tableau dashboard built from a synthetic dataset that simulates CRM, contacts, and deals data for a B2B sales organization. The goal is to showcase pipeline tracking, win rate analysis, and interactive filtering that mirror a real-world BI analyst workflow.

It is designed as a portfolio piece to demonstrate data preparation, schema modeling (Company–Contact–Deal relationships), dashboard design, and storytelling for stakeholders.

Folder Structure
tableau/
└── crm_db_pipeline-01/
    ├── data/
    │   ├── companies_dataset_raw.csv        (dimension table: companies)
    │   ├── contacts_dataset_raw.csv         (dimension table: contacts, includes internal + external)
    │   └── deals_dataset_raw.csv            (fact table: deals/pipeline)
    ├── workbook/
    │   └── crm_pipeline_dashboard.twbx      (Tableau packaged workbook)
    ├── CRM_pipeline_dashboard.pdf           (exported dashboard for review)
    └── README.txt                           (this file)

Dataset Details

companies_dataset_raw.csv
Synthetic dataset with 100 companies. Fields:
company_id, company_name, hq_country, hq_state, company_size, has_ever_been_subscribed, last_ended_subscription_date.

contacts_dataset_raw.csv
Unified contact dataset with both external (champion, lead, partner, former user) and internal (sales team) contacts. Fields:
contact_id, company_id, contact_type, firstname, lastname, email, campaign_ids, role, contact_owner.

deals_dataset_raw.csv
Synthetic fact table of deals tied to companies. Fields:
deal_id, company_id, stage, commit_date, status, days_in_stage, deal_owner, deal_size, probability.

Key KPIs

Pipeline Value (Active) = sum of deal size where status = Active

Closed Won Revenue = sum of deal size where status = Closed Won

Closed Lost Revenue = sum of deal size where status = Closed Lost

Win Rate (%) = closed won deals ÷ (closed won + closed lost)

Dashboard Features

KPI Cards: Pipeline Value, Closed Won, Closed Lost, Win Rate %

Funnel Visualization: Deal value by Stage (Active only)

Trend Analysis: Monthly Closed Won revenue with cumulative running total

Filters: Company Size, HQ Country, Subscription status, Stage, Status

Interactivity: Filters apply across all views; responsive to segment or lifecycle selection

Usage Instructions

Open the .twbx file in Tableau Public Desktop.

If needed, reconnect the dashboard to the CSVs in the data/ folder.

Explore interactively by applying filters for stage, company size, subscription, or geography.

For distribution, export the dashboard as PDF or Image and share with stakeholders, or publish to Tableau Public.

Purpose

This project is intended as a demonstration of CRM pipeline reporting and BI dashboarding skills.
It highlights the ability to:

Prepare and normalize synthetic CRM data (Companies, Contacts, Deals).

Model fact/dimension relationships in Tableau.

Build an executive-style dashboard that delivers actionable insights for sales leadership.

It can be reused as a template for similar CRM and sales analysis projects.