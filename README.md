# Mini Power BI Dashboard: Business Insights Case Study

A Power BI dashboard built to transform raw data into actionable business insights through data cleaning, modeling, DAX calculations, and interactive visualizations.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data%20Analysis%20Expressions-blue)
![Status](https://img.shields.io/badge/Status-Complete-success)

---

## Project Overview

This project demonstrates an end-to-end Power BI workflow, starting from raw data and ending with an interactive dashboard designed for business decision-making.

The objective was to identify trends, measure performance, and answer key business questions through data visualization and analytics.

The dashboard enables users to:

- Monitor KPIs
- Analyze category-level performance
- Identify top-performing segments
- Compare metrics across dimensions
- Generate actionable business insights

---

## Business Problem

Organizations often possess large volumes of raw data but lack a centralized reporting solution that converts data into meaningful insights.

This project addresses that challenge by:

- Cleaning and transforming raw data
- Building a structured data model
- Creating DAX measures for analysis
- Designing an interactive dashboard for stakeholders

---

## Dataset

The dataset contains information related to business performance and includes multiple dimensions used for analysis.

### Key Fields

- Category
- Sub-Category
- Product / Service Information
- Revenue Metrics
- Performance Metrics
- Customer Information
- Time-Based Data

---

## Data Preparation

### Power Query Transformations

- Removed unnecessary columns
- Handled null values
- Corrected data types
- Standardized text values
- Created calculated columns
- Optimized dataset structure

---

## Data Modeling

A star-schema inspired model was created to improve performance and maintainability.

### Relationships

- Fact Table
- Dimension Tables
  - Category
  - Date
  - Customer
  - Product

---

## DAX Measures

Several DAX measures were created to support dashboard analytics:

### KPI Measures

- Total Revenue
- Total Transactions
- Total Customers
- Average Performance
- Growth Percentage

### Advanced Calculations

- Ranking Measures
- Category-Level Analysis
- Percentage Contribution
- Running Totals
- Context-Aware Calculations using:

```DAX
CALCULATE()
ALL()
ALLEXCEPT()
RANKX()
```

---

## Dashboard Pages

### Home

Executive overview of the complete dashboard.

### Q1

Business question 1 analysis.

### Q2

Business question 2 analysis.

### Q3

Business question 3 analysis.

### Q4

Business question 4 analysis.

### Q5

Business question 5 analysis.

### Q6

Business question 6 analysis.

### Q7

Business question 7 analysis.

### Q8

Business question 8 analysis.

### Q9

Business question 9 analysis.

### Q10

Business question 10 analysis.

### Conclusion

Final recommendations and key insights.

---

## Key Insights

Some major findings generated from the dashboard include:

- High-performing categories drive the majority of business value.
- A small number of segments contribute disproportionately to overall results.
- Certain customer groups show significantly higher engagement.
- Performance varies across categories and dimensions.
- Data-driven prioritization opportunities were identified.

---

## Tools & Technologies

- Power BI Desktop
- Power Query
- DAX
- Data Modeling
- Interactive Visualizations

---

## Repository Structure

```text
├── Mini Power BI project.pbix
├── Dataset.csv
├── Screenshots/
└── README.md
```

---

## How to Explore

1. Download the repository.
2. Open the `.pbix` file using Power BI Desktop.
3. Refresh data if required.
4. Use slicers and filters to interact with the dashboard.
5. Navigate through all report pages for detailed analysis.

---

## Skills Demonstrated

- Data Cleaning
- Data Transformation
- Data Modeling
- DAX
- Business Intelligence
- Dashboard Design
- Data Visualization
- Analytical Thinking

---

## Future Improvements

- Real-time data integration
- Automated refresh pipelines
- Additional KPI tracking
- Predictive analytics
- Advanced forecasting models

---

## Author

**Aaryan Arora**

Business Analyst | Data Analyst | Power BI Developer

GitHub: https://github.com/Aaryan-2004-Arora

LinkedIn: <Your LinkedIn URL>
