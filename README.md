# Real-Time-Streaming-with-Azure-Databricks

## Project Overview
###Objective: Learn to build a data engineering pipeline utilizing Microsoft Fabric’s Data Factory, Data Engineering, and Power BI functionalities.

###Workflow:
####Data Ingestion: Utilize Python’s requests library to fetch raw data from the USGS API.
###Data Processing:
####Bronze Layer: Store raw data with minimal changes.
####Silver Layer: Clean and transform data for improved accuracy.
####Gold Layer: Refine data into business-ready datasets optimized for insights.
####Orchestration: Use Data Factory to automate daily data processing across the three layers.
###Reporting: Develop a Power BI report to visualize worldwide earthquake data.

###Technologies Used: Python, PySpark, Fabric (Data Engineering, Data Factory, Power BI)

## Getting Started
To get started with this project, clone the repository and follow the guidance provided in this YouTube tutorial.

## Repository Contents
- `Worldwide Earthquake Events API - Bronze Layer Processing`: This notebook focuses on ingesting raw earthquake data from the USGS API. It performs minimal processing to store data in its original format, serving as the foundational layer for further refinement.
- - `Worldwide Earthquake Events API - Silver Layer Processing`: This notebook enhances the data from the Bronze layer by cleaning, transforming, and consolidating the earthquake data. It prepares the data for more analytical processing.
- `Worldwide Earthquake Events API - Gold Layer Processing`: In this final processing stage, the notebook refines the data to create business-ready datasets. These are optimized for high-value insights and are tailored for specific analytical purposes, such as reporting and visualization in tools like Power BI.
- `data_attributes.txt`: Contains sample data and JSON structures for streaming simulation.
- `Solution Architecture.png`: High level solution architecture.

## Data Attribute Definitions
`id`: A string identifier for each data record.
`latitude`: The latitude of the event, stored as a double.
`longitude`: The longitude of the event, also stored as a double.
`elevation`: The elevation at which the event occurred, expressed in meters, stored as a double.
`title`: A string representing the title or name of the event.
`place_description`: A string describing the location of the event.
`sig`: A bigint (large integer) representing the significance score of the event.
`mag`: A double indicating the magnitude of the earthquake.
`magType`: A string describing the type of magnitude scale used.
`time`: A timestamp marking the exact time of the event.
`updated`: A timestamp indicating the last update time for the event data.

## Prerequisites
- Active Azure subscription with access to Azure Databricks and Event Hubs.
- Databricks Workspace with Unity Catalog Enabled.
- Azure Event Hubs Service.
- Power BI Desktop (Windows).
- Familiarity with Python, Spark, SQL, and basic data engineering concepts.
