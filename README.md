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

## Process

1. **Data Extraction:**
   - Utilized an SSIS package to read data from a CSV file.
   - Data was loaded into a staging table with necessary type conversions.
   
2. **Data Cleaning:**
   - Implemented checks to remove duplicate records.
   - Applied transformations to standardize data types and formats.
   - Error records were identified and handled appropriately.

3. **Incremental Loading:**
   - Designed a data flow to compare staging table data with the production table.
   - Inserted new records into the production table.
   - Updated existing records based on unique identifiers.

## Error Handling

- **Data Type Mismatches:**
  - Implemented data type checks and conversions during the transformation phase.
  
- **Duplicate Records:**
  - Applied deduplication logic to ensure unique records in the staging table.
  
- **Invalid Dates and Values:**
  - Utilized custom scripts to parse and correct invalid dates.
  - Handled erroneous values with default replacements or corrections.

## Outcomes

- Successfully migrated data from a CSV file to a SQL Server production table.
- Ensured data integrity through type standardization and error handling.
- Achieved efficient incremental loading with accurate identification of new and updated records.
- Demonstrated proficiency in SSIS-based ETL processes and data management techniques.
