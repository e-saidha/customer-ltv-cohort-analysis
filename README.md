# Customer Lifetime Value & Cohort Analysis

## Project Overview

This project analyzes customer purchasing behavior using the Online Retail II dataset.

The analysis combines:

- Cohort Retention Analysis
- Customer Lifetime Value (CLV) Modeling
- BG/NBD purchase prediction
- Gamma-Gamma monetary value modeling

The objective is to identify high-value customer segments and understand long-term retention behavior.

## Dataset

Online Retail II dataset from UCI Machine Learning Repository.

Customers analyzed: 5,878

Transactions analyzed: 805,549

## Business Questions

- What percentage of customers return after their first purchase?
- Which acquisition cohorts show the highest retention?
- Which customers are expected to generate the highest future revenue?
- How much future revenue is concentrated among top customers?

## Key Insights

- Top 10% of customers are predicted to generate approximately £4.39M of the projected £8.1M future revenue.
- Average Month-12 retention across mature cohorts is 16.4%.
- December acquisition cohorts generated approximately 2.5x higher customer lifetime value than non-December cohorts.
- Certain cohorts demonstrated increasing retention during early lifecycle stages.

## Methodology

### Data Cleaning

- Removed cancelled orders
- Removed negative quantities and prices
- Removed missing customer IDs

### Cohort Analysis

Customers were grouped by acquisition month and retention matrices were constructed.

### CLV Modeling

- BG/NBD model for purchase frequency prediction
- Gamma-Gamma model for monetary value prediction

## Technologies Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Lifetimes

## Future Improvements

- Add customer segmentation using RFM analysis
- Build an interactive dashboard using Power BI or Streamlit
- Deploy as a web application
