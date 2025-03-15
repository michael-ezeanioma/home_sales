# Overview

Leveraging Python, PySpark, and SparkSQL, this project analyzes home sales data to extract key metrics, optimize queries, and improve data processing efficiency. The project involves creating temporary views, partitioning data, caching tables, and comparing query performance using different optimizations.

# Project Components

__1. Data Preprocessing:__
Loads home_sales_revised.csv into a PySpark DataFrame while creating a temporary table (home_sales) for SQL-based querying.

__2. Data Analysis using SparkSQL:__
Calculates the average price of four-bedroom homes sold each year and homes built in different years with three bedrooms and three bathrooms. Evaluates prices for homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet, as well as home prices based on 'view' ratings for properties valued at $350,000 or more, including runtime evaluation.

__3. Performance Optimization:__ 
Caches the home_sales table and verifies its status, then runs queries on cached data to compare runtime with uncached queries. It partitions the data by date_built, creates a Parquet table, and reruns queries to evaluate efficiency. Once table is uncached, its removal from memory is verified.

# Files

__Home_Sales.ipynb:__ Jupyter Notebook containing all analysis and code.

__home_sales_revised.csv:__ Dataset for home sales analysis.

__Parquet files:__ Generated partitioned data for optimized querying.

# Key Features

__Data Preprocessing:__ Reads home sales data and extracts relevant variables and Creates a temporary SparkSQL table for efficient querying.

__SparkSQL Analysis:__ Executes SQL queries to extract home price trends and analyzes housing data based on key attributes like bedrooms, floors, and square footage.

__Performance Optimization:__ Implements caching to reduce query runtime. Uses Parquet partitioning to optimize data retrieval while comparing query performance across different optimization strategies.

# Dependencies

__PySpark:__ Enables large-scale data processing using SparkSQL.AWS 

__S3:__ Stores and retrieves the home sales dataset.

__Parquet:__ Optimized storage format for big data analytics.

# Technologies Used

__Python:__ Core programming language for data processing.

__PySpark & SparkSQL:__ Executes large-scale SQL queries.

__Jupyter Notebook:__ Interactive environment for running PySpark commands.

# How to Use

1 .Clone this repository to your local environment
2 .Install PySpark if not already installed
3. Open and run the Home_Sales.ipynb notebook in Jupyter Notebook or Google Colab.
4. Execute SQL queries, analyze trends, and compare query performance with different optimizations.
Module 22 HW
