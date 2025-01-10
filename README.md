# MicrosoftAzure
Project Overview

Data Ingestion
Source: NYC Taxi website

Method: Dynamic pipeline

Tool: Azure Data Factory

Output: Bronze file

Description: The data is ingested from the NYC taxi website using a dynamic pipeline configured in Azure Data Factory. The raw data is stored in a bronze layer for further processing.
Data Transformation


Service Principle: Azure Databricks

Process:
Transform data from the bronze layer to the silver layer.
Clean, enrich, and prepare the data for analysis.

Description: Using Azure Databricks, the data is transformed into a more structured format in the silver layer. This involves data cleaning, filtering, and enrichment to prepare it for further analysis.


Delta Lake Functions
Layer: Gold file

Functions Used:
Data Versioning: Maintain historical versions of the data for auditing and rollback purposes.

Time Travel: Query previous versions of the data to analyze changes over time.

Description: The gold layer leverages Delta Lake functionalities to provide robust data management capabilities, allowing users to track changes and revert to previous states of the data as needed.
Reporting


Tools: Power BI or Tableau
Purpose: Visualize and analyze the processed data for insights.

Description: After processing the data into the gold layer, Power BI or Tableau is used to create interactive dashboards and reports, enabling stakeholders to derive insights from the NYC taxi data.
