# Startup Hiring Monitor – Real-Time Signal Tracker for Growing Startups

## Project Overview

Startups actively hiring are often scaling, launching new products, or raising capital — making their hiring activity a powerful signal of business momentum.

Startup Hiring Monitor is a data-driven project designed to track growth signals from Indian startups based on their live job postings. This system scrapes, cleans, and analyzes open roles across startup career pages to extract actionable insights for investors, recruiters, and SaaS vendors.


## Objective

To build a signal tracker that identifies startup momentum using structured hiring data.


## What This Project Does

- Scrapes job postings from 10–15 Indian startup career pages

- Extracts structured fields: job title, department, location, job link, and scrape date

- Cleans and standardizes raw data for consistency

- Tags startups with growth signals based on hiring patterns (e.g., “Aggressive Engineering Hiring”, “New GTM Team”)

- Summarizes actionable insights from the data

- Presents data in CSV + PDF dashboard report format


## Tools & Technologies Used

| Task               | Tools Used                              |
| ------------------ | --------------------------------------- |
| Web Scraping       | `requests`, `BeautifulSoup`, `Selenium` |
| Data Cleaning      | `pandas`, `regex`, Jupyter Notebook     |
| Data Visualization | Power BI                |
| Reporting          | Notion                         |


## Repository Structure

```
.
├── Scraped_raw_data/
│   ├── Data_scraping.ipynb              - Jupyter notebook for scraping logic
│   └── raw_data.csv                     - Unprocessed scraped job data
│
├── Cleaned_data_with_tags/
│   ├── Data_cleaning.ipynb              - Data transformation, cleaning, and tagging logic
│   ├── Cleaned_data.csv                 - Cleaned dataset (without tags)
│   └── Cleaned_data_with_tags.csv       - Final dataset with growth signal tags
│
├── Startup_monitor_analysis_report.pdf  - Visual dashboard and summary insights
└── README.md                            - Project documentation
```

## Dataset Fields

| Column Name        | Description                                |
| ------------------ | ------------------------------------------ |
| `company_name`     | Name of the startup                        |
| `job_title`        | Role title (e.g., Backend Engineer)        |
| `department`       | Function/Team (e.g., Engineering, Sales)   |
| `location`         | Location (Remote/City-based)               |
| `url`              | Direct job posting link                    |
| `scrape_date`      | Date when the role was scraped             |


Growth Signal Tags – Examples

- Aggressive Engineering Hiring

- Remote Expansion

- New GTM Team

- Company-wide Scaling

- Possible Hiring Freeze (if no active jobs)


## Insight Summary

- **Drip Capital** is undergoing a broad-scale hiring push with **14 open roles** across 5+ departments - a strong signal of **Company-Wide Scaling**.

- **Groww** is aggressively hiring for **product and engineering teams**, with multiple PM roles -indicates a **New Product Buildout** and strategic expansion.

- **Chargebee** shows a clear **GTM Team Expansion**, driven by **3+ Sales roles** and roles in Customer Support and Marketing.

- **CRED** has limited hiring activity (only 4 roles), concentrated in operations and marketing -suggesting a **steady-state team** with no aggressive scaling.

- **Meesho** has **15 active roles**, mostly in **Operations**, with low presence in tech/product - possibly investing in logistical backbone rather than core product growth.

- **Paytm** (based on full data, assuming further entries) likely shows balanced hiring across Product, Data, and Design - aligned with **product-focused growth** strategy.

- None of the startups demonstrate a **Remote Hiring Focus**, as remote roles are minimal or absent across the board.

- The **Engineering Push** is visible in **Groww** and Meesho, though still modest compared to PM and Ops roles - could suggest mature tech teams or outsourced builds.

- **Legal and Compliance** roles appear clustered in Drip Capital - possibly due to regulatory oversight in fintech-heavy operations.

- **Chargebee’s** mixed hiring in support, product, and sales indicates a **customer-centric scaling approach**, likely aiming at customer success and churn control.


## Final Deliverables

- Cleaned, tagged dataset (cleaned data with tags.csv)

- Insight dashboard (startup monitor analysis report.pdf)

- Raw data and code notebooks (.ipynb files)

- Growth signal summary (in report)


## Who This Is For

- Investors looking to track early signals of startup growth

- Recruiters targeting fast-growing companies

- SaaS vendors identifying potential B2B leads
