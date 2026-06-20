# Recorded Lectures, Decoded: An EdTech Power BI Case Study

A Power BI dashboard built to transform raw EdTech course data into actionable business insights. This project analyzes learner engagement, course performance, language preferences, instructor quality, skill demand, and content accessibility to help an EdTech startup make data-driven decisions for expanding its recorded lecture offerings.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-CALCULATE%20%7C%20RANKX%20%7C%20ALLEXCEPT-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Transformation-success)
![Status](https://img.shields.io/badge/Status-Complete-success)

---

# The Business Problem

An EdTech startup aims to expand its recorded lecture business but lacks visibility into learner preferences, content performance, instructor effectiveness, and language demand.

The company collected data from multiple EdTech platforms but needed a structured analysis to answer critical business questions regarding:

- Which categories attract the most learners?
- Which course formats perform best?
- Which skills are currently in demand?
- Which languages should future courses support?
- Do subtitles increase engagement?
- Which instructors should the company partner with?
- What course duration attracts the highest viewership?

A major project requirement was that all analysis should be performed with a **Category-First Approach**, allowing stakeholders to evaluate performance at both Category and Sub-Category levels.

---

# Project Objectives

The dashboard was developed to answer the following business questions:

| # | Business Question |
|---|---|
| Q1 | Examine the distribution of course types across categories and sub-categories. |
| Q2 | Calculate average views for each category, sub-category, and language. |
| Q3 | Identify the most commonly taught skills by category. |
| Q4 | Analyze the distribution of languages in which courses are created. |
| Q5 | Determine language preferences for the Top 5 categories based on viewer demand. |
| Q6 | Investigate the relationship between subtitle availability and viewer engagement. |
| Q7 | Identify the Top 3 instructors for each category and sub-category based on ratings. |
| Q8 | Examine the relationship between course duration and number of views. |
| Q9 | Analyze whether skill diversity influences viewership. |
| Q10 | Generate strategic recommendations for future course investments. |

---

# Dataset Overview

The dataset contains information collected from multiple online learning platforms and includes:

### Course Information

- Course Name
- Course Type
- Category
- Sub-Category

### Engagement Metrics

- Number of Viewers
- Ratings

### Content Attributes

- Duration
- Language
- Subtitle Languages
- Skills Covered

### Instructor Information

- Instructor Name(s)

The raw dataset contained several multi-value fields where a single course could have multiple instructors, skills, or subtitle languages.

---

# Data Cleaning & Transformation

The data preparation process was performed entirely in **Power Query**.

### Key Cleaning Steps

- Removed unnecessary and sparse columns
- Handled missing values
- Standardized text formatting
- Converted ratings into numerical values
- Converted viewer counts into numerical format
- Standardized duration values

### Duration Transformation Logic

To ensure consistency:

| Original Value | Converted To |
|---------------|-------------|
| 1 Month | 60 Hours |
| Flexible Schedule | 200 Hours |

### Multi-Value Field Handling

The following columns contained comma-separated values:

- Skills
- Instructors
- Subtitle Languages

Separate analytical tables were created to properly analyze these dimensions without causing aggregation issues.

---

# Data Modeling

A relational model was created to support accurate reporting and analysis.

### Main Analytical Dimensions

- Category
- Sub-Category
- Skills
- Language
- Subtitle Languages
- Instructors

This approach allowed:

- Accurate aggregations
- Instructor ranking analysis
- Skill frequency analysis
- Subtitle impact analysis
- Language preference analysis

without double-counting courses.

---

# DAX Measures & Calculations

The dashboard uses several DAX functions to perform advanced business analysis.

### Core Functions Used

```DAX
CALCULATE()
ALL()
ALLEXCEPT()
RANKX()
COUNTROWS()
AVERAGEX()
DISTINCTCOUNT()
```

### Key Measures

- Total Courses
- Total Views
- Average Views
- Average Rating
- Course Count by Category
- Course Count by Sub-Category
- Top Instructor Ranking
- Language Ranking
- Skill Frequency
- Skill Diversity Metrics

---

# Dashboard Analysis

## Q1 — Course Type Distribution

### Objective

Analyze how different course types are distributed across categories and sub-categories.

### Insights Generated

- Course count by category
- Course count by sub-category
- Course type distribution
- Popular content formats

### Business Value

Helps determine which course formats should be launched within specific categories.

---

## Q2 — Viewer Engagement Analysis

### Objective

Calculate average views across:

- Categories
- Sub-Categories
- Languages

### Insights Generated

- High-engagement categories
- High-engagement sub-categories
- Language-wise viewer behavior

### Business Value

Helps prioritize investments in categories with the highest learner demand.

---

## Q3 — Skill Demand Analysis

### Objective

Identify the most commonly taught skills in each category.

### Insights Generated

- Top skills by category
- Skill frequency rankings
- Emerging learning trends

### Business Value

Ensures future course offerings remain aligned with industry demand and learner interests.

---

## Q4 — Language Distribution Analysis

### Objective

Understand the language distribution of courses.

### Insights Generated

- Language share across the catalog
- Dominant course languages
- Localization opportunities

### Business Value

Supports content expansion into underserved language markets.

---

## Q5 — Language Preference Analysis

### Objective

Analyze viewer language preferences within the Top 5 categories.

### Insights Generated

- Top-performing languages
- Language popularity by category
- Viewer demand patterns

### Business Value

Guides future content localization strategies.

---

## Q6 — Subtitles vs Viewer Engagement

### Objective

Determine whether subtitle availability impacts viewership.

### Insights Generated

- Subtitle count distribution
- Average views by subtitle coverage
- Accessibility impact analysis

### Business Value

Measures the ROI of investing in multilingual subtitles.

---

## Q7 — Top Instructor Analysis

### Objective

Identify the Top 3 instructors for each category and sub-category based on ratings.

### Insights Generated

- Instructor rankings
- High-performing educators
- Category-specific teaching leaders

### Business Value

Provides a shortlist of instructors who can be approached for partnerships and content creation.

---

## Q8 — Duration vs Viewership Analysis

### Objective

Understand how course duration impacts viewer engagement.

### Insights Generated

- Duration patterns
- Optimal course lengths
- Engagement by category and sub-category

### Business Value

Helps design courses with durations that maximize learner retention and viewership.

---

## Q9 — Skill Diversity Impact Analysis

### Objective

Investigate whether the variety of skills offered influences course popularity.

### Insights Generated

- Skill count by category
- Skill diversity vs average views
- Breadth of learning opportunities

### Business Value

Helps determine whether broader skill coverage increases learner engagement.

---

## Q10 — Strategic Recommendations

### Objective

Combine findings from all analyses into actionable recommendations.

### Recommendations Focus On

- Category Expansion
- Language Strategy
- Subtitle Investments
- Instructor Partnerships
- Skill-Based Content Planning
- Optimal Course Design

---

# Key Findings

### Category Matters Most

Certain categories consistently attract higher viewership and engagement, making them prime candidates for future investment.

### Skills Drive Demand

Frequently taught and industry-relevant skills attract significantly higher learner interest.

### Language Influences Reach

English dominates the catalog, but localized content presents a significant growth opportunity.

### Subtitles Improve Accessibility

Courses with broader subtitle coverage tend to achieve stronger engagement.

### Instructor Quality Impacts Success

A small group of instructors consistently receive top ratings across multiple categories.

### Duration Has an Effect

Both short-form and well-structured long-form content outperform average-length courses.

### Skill Diversity Can Increase Engagement

Courses offering broader skill coverage often attract more viewers and create greater learner value.

---

# Tools & Technologies

### Business Intelligence

- Power BI Desktop

### Data Preparation

- Power Query

### Data Modeling

- Star Schema Principles
- Relationship Modeling

### Analytics

- DAX

### Visualization

- Interactive Dashboards
- Slicers
- Drilldowns
- Tooltips
- Ranking Visuals

---

# Repository Structure

```text
├── Mini Power BI project.pbix
├── Online_Courses.csv
├── Screenshots/
│   ├── Home.png
│   ├── Q1.png
│   ├── Q2.png
│   ├── Q3.png
│   ├── Q4.png
│   ├── Q5.png
│   ├── Q6.png
│   ├── Q7.png
│   ├── Q8.png
│   ├── Q9.png
│   ├── Q10.png
│   └── Conclusion.png
└── README.md
```

---

# How To Explore

1. Clone this repository.
2. Open `Mini Power BI project.pbix` using Power BI Desktop.
3. Refresh data if required.
4. Navigate through dashboard pages.
5. Use slicers and filters to explore category-level insights.
6. Drill into categories and sub-categories for deeper analysis.

---

# Skills Demonstrated

- Data Cleaning
- Data Transformation
- Power Query
- Data Modeling
- DAX
- Business Analysis
- Dashboard Development
- Data Visualization
- Insight Generation
- Stakeholder Reporting
- KPI Design
- Analytical Thinking

---

# Future Improvements

With additional data, the analysis could be extended to include:

- Time-Series Engagement Trends
- Revenue Analysis
- Course Pricing Analysis
- Learner Retention Metrics
- Predictive Demand Forecasting
- Recommendation Systems

---

# Author

## Aaryan Arora

Business Analyst | Data Analyst | Power BI Developer

### Connect With Me

- GitHub: https://github.com/Aaryan-2004-Arora
- LinkedIn: https://www.linkedin.com/in/aaryan-arora

---

If you found this project useful, consider giving the repository a ⭐.
