# Azure Data Engineering Project :rocket:

Build an end-to-end pipeline to copy data from the on-premises SQL Server to Azure blob storage using ADF.

![image](https://github.com/Rakesh-Pawar/Azure-Data-Enginering-Project/assets/112051343/4160242f-9d3b-4da9-9603-9aae02c99372)


## Table of Contents

- [:mag: Project Overview](#project-overview)
- [:floppy_disk: Data Source](#data-source)
- [:wrench: Tools Used](#tools-used)
- [:bulb: Use Case](#use-case)
- [:gear: Project Process](#project-process)

## :mag: Project Overview

The use case for this project is building an end-to-end solution by ingesting the tables from the on-premise SQL Server database using Azure Data Factory and then storing the data in Azure Data Lake. Then Azure Databricks is used to transform the RAW data to the cleanest form of data. Finally, we use Azure Synapse Analytics to load the clean data, and Microsoft Power BI to integrate with Azure Synapse Analytics to build an interactive dashboard.

## :floppy_disk: Data Source

- **Source**: On-premise SQL Server Database. Download data and restore on SQL server [AdventureWorksLT2017](https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorksLT2017.bak)
- **Destination**: Azure SQL

## :wrench: Tools Used

This project makes use of the following tools:

1. :cloud: [Azure Data Factory](https://azure.microsoft.com/en-us/services/data-factory/)
2. :file_folder: [Azure Data Lake Storage Gen2](https://azure.microsoft.com/en-us/services/storage/data-lake-storage/)
3. :bar_chart: [Azure Databricks](https://azure.microsoft.com/en-us/services/databricks/)
4. :rocket: [Azure Synapse Analytics](https://azure.microsoft.com/en-us/services/synapse-analytics/)
5. :chart_with_upwards_trend: [Microsoft Power BI](https://powerbi.microsoft.com/)

## :bulb: Use Case

The project's use case involves the following steps:

- :arrow_forward: **Step 1**: Data is initially stored in an on-premise SQL Server database.
- :arrows_counterclockwise: **Step 2**: Azure Data Factory (ADF) is employed for extracting and loading data from the on-premise database to the Azure cloud.
- :file_folder: **Step 3**: Extracted data is stored in Azure Data Lake Storage (ADLS) Gen2 for scalable, secure storage.
- :hammer_and_wrench: **Step 4**: Azure Databricks is utilized to perform data transformations, making it cleaner and more usable.
- :globe_with_meridians: **Step 5**: Azure Synapse Analytics processes the refined data, producing a "gold" dataset.
- :chart_with_downwards_trend: **Step 6**: Microsoft Power BI connects to Azure Synapse Analytics, creating interactive reports and dashboards for end-users.


## Project Process :hammer_and_wrench:

The project involves a well-defined process, which can be broken down into the following key steps:

### :file_folder: Data Source
Data is initially stored in an on-premise SQL Server database. This database serves as the foundational data repository, housing crucial business information.

### :arrows_counterclockwise: Data Movement
Azure Data Factory (ADF) is harnessed for data movement. ADF orchestrates the extraction and loading of data from the on-premise database to the Azure cloud. This step is vital for ensuring data continuity.

### :file_folder: Data Storage
Extracted data finds its home in Azure Data Lake Storage (ADLS) Gen2. ADLS offers scalable and cost-effective data storage, providing a structured yet flexible environment for large datasets.

### :bar_chart: Data Transformation
Azure Databricks takes the stage for data transformation. This transformative phase includes various critical tasks:
- :broom: Data Cleansing: Removing duplicates, handling missing values, and ensuring data consistency.
- :chart_with_upwards_trend: Data Enrichment: Augmenting data with additional information.
- :twisted_rightwards_arrows: Data Transformation: Shaping data to meet specific business requirements, including aggregation and summarization.
- :telescope: Advanced Analytics: Applying advanced analytics techniques such as machine learning and statistical analysis to extract insights from the data.

### :gear: Data Processing
Azure Synapse Analytics leads the way for data processing. This comprehensive phase involves essential components:
- :building_construction: Data Warehousing: Organizing and structuring data for efficient querying and reporting.
- :rocket: Big Data Analytics: Leveraging the power of big data processing for handling massive datasets and complex analytical workloads.
- :link: Data Integration: Integrating data from various sources to ensure consistency and reliability. Data from different sources is combined to create a comprehensive view of the business data.

### :chart_with_upwards_trend: Reporting and Visualization
Microsoft Power BI connects to Azure Synapse Analytics, enabling the creation of interactive reports and dashboards for end-users. Power BI empowers users to:
- :mag: Explore and Visualize Data: Create custom reports and visualizations to gain insights.
- :speech_balloon: Share Insights: Share reports and dashboards with team members and stakeholders.
- :chart: Make Data-Driven Decisions: Enable users to make informed decisions based on the processed and visualized data, enhancing business intelligence.

