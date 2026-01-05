# Cloud-based Agriculture Analytics Dashboard
An end-to-end cloud analytics project integrating AWS, Snowflake, and Power BI to analyze the impact of climate factors (rainfall, temperature, humidity) on agricultural yield.

## Dashboard Link
https://app.powerbi.com/groups/me/reports/d23e9636-76fe-40d5-a0bc-3c442dc2e604/73dfaf0ce1d8c2328a90?experience=power-bi

## Project Overview
* Raw agricultural & climate data is stored securely in AWS S3
* Data is ingested, transformed, and modeled in Snowflake
* Insights are visualized through Power BI dashboards

## Security Design
* No hardcoded credentials
* AWS IAM Role-based access with STS AssumeRole
* Optional External ID to prevent confused-deputy attacks
* Snowflake role-based access control (RBAC)
* Power BI uses controlled Snowflake authentication

## Tech Stack
* Cloud Storage: AWS S3
* Security: AWS IAM, STS
* Data Warehouse: Snowflake
* BI & Analytics: Power BI
* Language: SQL, DAX

## Power BI Dashboard Pages
* Rainfall Analysis – Trend & regional rainfall patterns
* Temperature Analysis – Seasonal & average temperature insights
* Humidity Analysis – Risk & correlation analysis
* Yield Analysis – Productivity trends & comparisons

## How to Run This Project
* Upload raw data files to AWS S3
* Configure IAM Role & Trust Policy
* Create Snowflake stages and load data using **COPY INTO**
* Transform data in Snowflake tables/views
* Connect Power BI to Snowflake
* Refresh data & publish report

## Contributing Guidelines
Contributions are welcome!
* Fork the repository
* Create a feature branch
  ``` git checkout -b feature/your-feature-name ```
* Commit changes with clear messages
* Push to your fork
* Open a Pull Request

## Learning Outcomes
* Designing secure cross-cloud architectures
* Snowflake data modeling & ingestion
* Power BI semantic modeling
* Cloud security best practices
* End-to-end analytics pipeline

## License
No license

## Acknowledgement
Built as a learning and portfolio project to demonstrate Cloud + Data Analytics integration.
