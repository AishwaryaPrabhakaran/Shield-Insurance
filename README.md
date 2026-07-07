# 🛡️ Shield Insurance – Sales & Customer Intelligence Dashboard (FY 2022–2023)

A Power BI dashboard designed to help Shield Insurance monitor revenue performance, customer behavior, sales channel effectiveness, and settlement patterns across cities and age groups.

This project focuses on transforming raw insurance data into actionable business insights through data modeling, DAX calculations, and interactive dashboard storytelling.

---

## 📌 Project Overview

The objective of this project was to create a business-friendly reporting solution that enables stakeholders to:

- Track revenue and customer growth trends
- Understand channel performance across cities
- Analyze customer behavior by age group
- Identify settlement patterns across demographics
- Support data-driven decision-making through intuitive visualizations

---

# 🏗️ Project Workflow

## 1️⃣ Data Connection

Connected multiple source files from the provided dataset folder into Power BI.

The datasets included:

- Customer Information
- Premium Transactions
- Settlement Data
- Policy Information

---

## 2️⃣ Data Transformation (Power Query)

Several transformations were performed to improve data quality and usability.

### Customer Data

- Removed unnecessary columns
- Validated customer age values
- Created Age Group buckets

Example:

| Age | Age Group |
|------|-----------|
| 22 | 18–24 |
| 29 | 25–30 |
| 37 | 31–40 |
| 45 | 41–50 |
| 58 | 51–65 |
| 70 | 65+ |

---

### Date Table Creation

Created a dedicated Date Dimension to support time intelligence calculations.

Additional columns created:

- Month Name
- Week Number
- Day Type
- MMM_YY

Example:

| Date | MMM_YY |
|--------|---------|
| 2022-11-01 | Nov_22 |
| 2023-01-01 | Jan_23 |

---

### Sorting Month-Year Correctly

A custom YearMonthSort column was created to prevent alphabetical sorting issues.

Example:

| MMM_YY | YearMonthSort |
|---------|---------------|
| Nov_22 | 202211 |
| Dec_22 | 202212 |
| Jan_23 | 202301 |

MMM_YY was then sorted using YearMonthSort.

---

### Additional Columns Created

- Age Group
- YearMonthSort
- Day Type
- Day Number (for weekday sorting)

---

# 🗂️ Data Modeling

A star-schema model was implemented.

### Dimension Tables

- dim_customer
- dim_date
- dim_policies

### Fact Tables

- fact_premiums
- fact_settlements

### Supporting Tables

- Parameter Table
- Bridge Table

The model was designed to support:

- Time Intelligence
- Customer Segmentation
- Sales Channel Analysis
- Settlement Analysis

---

# 📊 DAX Measures

Several DAX measures were created to drive insights and KPIs.

Examples include:

- Revenue
- Customer Count
- Average Settlement %
- Previous Month Revenue
- Revenue Growth %
- Daily Revenue
- Daily Customer Count
- Dynamic KPI Measures
- Insight Card Measures

📄 A detailed list of DAX measures is documented separately and can be found in:

```
DAX_Measures_Documentation.md
```

---

# 🎨 Dashboard Design Approach

Before creating visuals, a custom report theme was designed based on the Shield Insurance branding.

### Design Principles

- Consistent color palette derived from company logo
- Dark theme for improved contrast
- Minimal visual clutter
- Executive-friendly layout
- Guided storytelling approach
- Consistent navigation across pages

The report follows a structured navigation flow:

```
Homepage
    ↓
Overview
    ↓
Sales Mode Analysis
    ↓
Age Group Analysis
```

---

# 🏠 Homepage

The homepage acts as a navigation hub and executive summary.

### Key Features

✅ Executive KPIs at a glance

✅ Top-performing sales channel

✅ Highest settlement age group

✅ Navigation buttons to analytical pages

✅ High-level business insights

### Snapshot

*(Add Homepage Screenshot Here)*

---

# 📈 Overview Page

The Overview page answers the fundamental business questions.

### Business Questions

- How much revenue are we generating?
- Which cities contribute the most revenue?
- Which customer segments drive business performance?
- How are revenue and customer trends changing month-over-month?

### Visuals Included

- Revenue KPI
- Customer KPI
- Daily Revenue KPI
- Daily Customer KPI
- Monthly Trend Analysis
- Revenue & Customer Split by City
- Revenue & Customer Split by Age Group
- Customer Segmentation Table

### Snapshot

*(Add Overview Screenshot Here)*

---

# 📡 Sales Mode Analysis

This page focuses on channel effectiveness and customer acquisition.

### Business Questions

- Which sales channel drives the most revenue?
- Which channel acquires the most customers?
- Which channels dominate in each city?
- How do sales patterns vary by day of week?

### Visuals Included

- Customer Count by Sales Mode
- Revenue Split Across Sales Modes
- Monthly Revenue Trend by Channel
- City-wise Sales Mode Preference
- Sales Mode Ranking by Day Type
- Dynamic Insight Panel

### Snapshot

*(Add Sales Mode Analysis Screenshot Here)*

---

# 👥 Age Group Analysis

This page explores customer behavior across age segments.

### Business Questions

- Which age group generates the most revenue?
- Which age group has the highest settlement rate?
- Which policies are preferred by each age segment?
- How do age groups differ in sales channel preference?

### Visuals Included

- Average Settlement % by Age Group
- Sales Mode Preference by Age Group
- Trend Chart by Age Group
- Policy Preference Heatmap
- Customer Count by Age Group

### Snapshot

*(Add Age Group Analysis Screenshot Here)*

---

# 💡 Key Insights

### Revenue & Customer Performance

- Revenue reached **₹989M**
- Customer count exceeded **27K**
- Revenue grew **18.4% compared to the previous month**

### Sales Mode Insights

- Offline-Agent contributes more than **56% of total revenue**
- Offline-Agent remains the dominant acquisition channel
- Weekends show significantly higher sales activity

### Geographic Insights

- Delhi NCR contributes the highest revenue
- Delhi NCR leads customer acquisition across channels

### Age Group Insights

- Customers aged **65+** show the highest settlement percentage (**74.3%**)
- Customers aged **31–40** represent the largest customer segment
- Policy preferences vary noticeably across age groups

---

# 🚀 Future Enhancements

Planned improvements:

- Dashboard walkthrough video
- Mobile-optimized layout
- Advanced tooltip pages
- Automated insights generation
- Drill-through analysis pages

---

# 🎥 Dashboard Walkthrough

A detailed dashboard walkthrough video will be added soon.

**Coming Soon**

```
[Dashboard Walkthrough Video Link]
```

---

# 🛠️ Tools & Technologies

- Power BI Desktop
- Power Query
- DAX
- Data Modeling
- Star Schema Design
- Interactive Navigation
- Custom Report Themes

---

# 🔗 Live Dashboard

View the report here:

https://app.powerbi.com/view?r=eyJrIjoiN2JmODljYjEtNDRkZC00M2Y0LTk2ZWMtYTE0OGUwNjk1ZDBmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9

---

# 👩‍💻 Author

**Aishwarya Prabakaran**

Aspiring Data Analyst | Power BI | SQL | Python | Databricks

Always open to feedback and suggestions for improving dashboard design, storytelling, and analytics.
