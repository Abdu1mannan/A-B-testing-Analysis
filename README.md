A/B Testing Analysis: Landing Page Conversion Optimization

Project Overview

End-to-end A/B testing analysis evaluating the impact of a redesigned landing page on conversion rates. This project demonstrates proficiency in SQL data modeling, statistical hypothesis testing, business intelligence visualization, and stakeholder communication.

Business Problem

Objective: Determine whether a new landing page design (Variant B) significantly improves conversion rates compared to the control (Variant A).

Key Metrics:
- Primary: Conversion Rate
- Secondary: CTA Click Rate, Revenue per Session

Technical Stack

- Database: PostgreSQL
- Analysis: Microsoft Excel (t-tests, confidence intervals)
- Visualization: Power BI

Data Architecture

Implemented a star schema with the following structure:
- Fact Tables: sessions, conversions
- Dimension Tables: users, experiment_assignment
- Analytical Tables: testing_table, revenue_dist

Key Findings

Overall Results
- Conversion Rate Uplift: +3.80% (12.58% to 16.37%)
- Revenue Uplift: $17,027.68 (+30.19% relative increase)
- Statistical Significance: Confirmed (p < 0.05)
- 95% Confidence Interval: [+2.43% to +5.17%]

Segment Insights
- Top Performing Country: United States (+4.77% conversion uplift)
- Top Performing Device: Tablet (+13% conversion uplift)
- Best Acquisition Channel: Paid (1,385 conversions)

Behavioral Metrics
- Average Session Duration: 4.24 minutes (identical across variants)
- CTA Click Rate: 43.45% (B) vs 40.16% (A)
- Pages per Session: 3.31

Methodology

1. Data Collection and Preparation (SQL)
Created relational database schema with proper foreign key relationships. Imported 10,200 user sessions across 90-day test period and built aggregation tables for analysis efficiency.

2. Statistical Analysis (Excel)
Conducted two-sample t-test for conversion rates. Calculated confidence intervals and p-values. Performed revenue distribution analysis using chi-square test. Revenue uplift not statistically significant (t = 0.48).

3. Visualization and Reporting (Power BI)
Developed interactive dashboard with four views: Executive Summary, Behavioral Analysis, Segment Analysis, and A/B Testing Overview.

Project Structure

A-B-testing/
├── Raw data files/
│   ├── conversions.csv
│   ├── experiment_assignment.csv
│   ├── revenue_dist.csv
│   ├── sessions.csv
│   ├── users.csv
│   └── Test_table.txt
├── Excel analysis-Hypothesis Testing.csv
├── Dashboard_A-B.pbix
└── Screenshots/
    ├── Behavioral Analysis.png
    ├── Executive Summary(a-b analysis).png
    ├── Segment Analysis.png
    ├── Excel Analysis (hypothesis testing).png
    ├── sql_tables_creation_for_tests.png
    └── table_star_schema.png

Recommendations

Deploy Variant B: Statistically significant improvement in conversion rate justifies full rollout.

Optimize for Mobile: Despite strong tablet performance, mobile shows conversion decline in some markets.

Leverage Paid Channels: Highest conversion volume suggests opportunity for increased investment.

Tools used:

SQL database design and querying (PostgreSQL), statistical hypothesis testing and A/B test analysis, data visualization and dashboard design (Power BI), business metrics interpretation and stakeholder communication, end-to-end analytics project execution.
