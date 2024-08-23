# Google Play Store Data Analysis

## Table of Contents
- Project Overview
- Data Description
- ETL Pipeline
- Data Transformation
- Data Analysis
- Technologies Used


## Project Overview
This project involves analyzing Google Play Store data using PySpark within Databricks. The objective is to clean, transform, and analyze the dataset to derive meaningful insights into app performance, category trends, and pricing.

## Data Description
The dataset used in this project is a CSV file containing information about various apps available on the Google Play Store. Key fields include:

- **App:** Name of the app
- **Category:** Category of the app
- **Rating:** App rating
- **Reviews:** Number of reviews
- **Installs:** Number of installs
- **Price:** Price of the app
- **Type:** Free or Paid

## ETL Pipeline
The ETL pipeline for this project is implemented in Databricks using PySpark. The pipeline includes:

- **Extraction:** Loading data from the CSV file located at `/FileStore/tables/googleplaystore.csv`.
- **Transformation:**
  - Dropping unnecessary columns.
  - Cleaning and casting data types (e.g., converting Installs and Price to integers).
  - Handling missing or incorrect values.
- **Loading:** Creating a temporary SQL view for analysis.

## Data Transformation
Data transformation steps include:

- Removing non-numeric characters from the Installs and Price fields.
- Converting Reviews, Installs, and Price fields to integer types.
- Dropping columns that are not needed for the analysis.

## Data Analysis
The analysis involved several key steps:

- **Top Reviews Given to the Apps:** Aggregated data to find the top apps by number of reviews.
- **Top 10 Install Apps:** Identified the top 10 apps based on the number of installs.
- **Top 10 Install Apps with Type:** Analyzed the top 10 apps by installs, segmented by app type (Free or Paid).
- **Category Wise Distribution:** Investigated the distribution of installs across different app categories.
- **Top Paid Apps:** Calculated total revenue from paid apps.

## Technologies Used
- **Databricks:** Cloud-based data analytics platform.
- **PySpark:** Python API for Apache Spark.
- **Spark SQL:** SQL querying on large datasets.


