# SSIS-ETL-Task

## Abstract

This repository contains an SSIS-based ETL solution designed to demonstrate data extraction, transformation, cleaning, and incremental loading capabilities. The task involves migrating data from a CSV file to a SQL Server production table via a staging table. Key operations include data type standardization, duplicate removal, error handling, and updating records based on unique identifiers. The solution simulates a real-world scenario with potential data errors, showcasing skills in data management and ETL process optimization.

## Objectives

- **Data Extraction and Type Standardization to Staging Table:**
  - Extract data from a CSV file using an SSIS package.
  - Transform and load the data into a staging table, converting string values to appropriate SQL data types (int, string, float, date, etc.).
  
- **Data Cleaning in Staging Table:**
  - Perform data cleaning operations including removing duplicates and handling error records.
  
- **Incremental Load to Production Table:**
  - Ensure the production table includes an ID column for unique record identification.
  - Create a data flow from the staging table to the production table, differentiating new from existing records based on ID.
  - Insert new records and update existing records.
