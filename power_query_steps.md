# Power Query Data Cleaning Steps

This document describes the data transformation steps applied using Power Query (M code).

## 1. Data Import
- Imported Excel file using `Excel.Workbook`
- Selected **Data Professional Survey** sheet
- Promoted first row as headers

## 2. Data Type Standardization
- Converted date and time columns
- Converted satisfaction ratings to numeric values

## 3. Column Removal
Removed irrelevant columns:
- Browser
- OS
- City
- Country
- Referrer

## 4. Job Title Cleaning
- Split job title column at "("
- Retained the main role title

## 5. Programming Language Cleaning
- Split values at ":"
- Kept primary programming language only

## 6. Salary Processing
- Duplicated salary column
- Split salary ranges
- Removed symbols (k, +, -)
- Converted to numeric values
- Calculated **Average Salary**

## 7. Country & Industry Cleaning
- Removed additional text in brackets
- Standardized naming

## 8. Final Output
- Removed intermediate columns
- Renamed columns for clarity
- Loaded cleaned data for analysis in Power BI
