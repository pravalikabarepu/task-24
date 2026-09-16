# Superstore Data Quality Audit

## Project Overview

This project performs a data quality audit on the Superstore dataset using Python. The objective is to identify missing values, duplicate records, range violations, and consistency issues through a repeatable validation checklist.

The audit produces an issue log with the quantity of each identified issue and creates a cleaned version of the dataset.

## Objective

Audit the Superstore dataset for common data quality problems and create a repeatable process for validating and cleaning the data.

## Tools Used

Python
Pandas
NumPy
Jupyter Notebook

## Dataset

Superstore dataset containing information about orders, customers, products, sales, quantity, discount, profit, and dates.

## Data Quality Checks

The following validation rules were applied:

1. Missing value check
2. Duplicate row check
3. Negative sales check
4. Invalid quantity check
5. Invalid discount check
6. Missing profit check
7. Invalid order date check
8. Invalid ship date check
9. Order date and ship date consistency check
10. Missing customer ID check

## Validation Rules

Sales should not be negative.

Quantity should be greater than zero.

Discount should be between 0 and 1.

Order Date should contain valid dates.

Ship Date should contain valid dates.

Ship Date should not be earlier than Order Date.

Customer ID and Profit should not be missing.

Duplicate records should be identified and removed.

## Deliverables

### Audit Report

Contains each validation rule, description, number of issues found, and PASS or FAIL status.

### Issue Log

Lists the validation rules where data quality issues were detected along with the issue count.

### Missing Value Report

Shows columns containing missing values and their respective counts.

### Range Report

Shows minimum, maximum, and invalid counts for important numerical fields.

### Cleaned Sample

Contains the first 100 records from the cleaned dataset.

### Cleaned Dataset

Contains the processed Superstore dataset after applying the defined cleaning rules.

## Cleaning Process

Duplicate records were removed.

Records with invalid sales values were removed.

Records with invalid quantity values were removed.

Records with discount values outside the range of 0 to 1 were removed.

Records where Ship Date occurred before Order Date were removed.

## Key Outcome

The project provides a repeatable Python-based data quality checklist that can be reused for similar datasets. It helps identify data issues before performing further analysis or building dashboards.

## Files

superstore_audit_report.csv

superstore_issue_log.csv

superstore_missing_report.csv

superstore_range_report.csv

superstore_cleaned_sample.csv

superstore_cleaned.csv

superstore_data_quality_audit.ipynb
