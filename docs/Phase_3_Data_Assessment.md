# Phase 3 – Data Assessment & Profiling

## Objective

The objective of this phase was to evaluate the quality, completeness, and structure of the available datasets before performing data cleaning and business analysis.

This assessment helps identify potential data quality issues that could affect downstream analysis.

---

# Activities Performed

The following assessment activities were completed:

- Loaded all datasets
- Generated dataset inventory
- Examined dataset dimensions
- Assessed memory usage
- Reviewed column information
- Validated data types
- Identified missing values
- Checked duplicate records
- Generated descriptive statistics
- Generated categorical summaries

---

# Dataset Summary

A total of nine datasets were assessed.

The analysis included:

- Number of rows
- Number of columns
- Memory consumption
- Data types
- Null values
- Duplicate records
- Numeric statistics
- Categorical statistics

---

# Key Findings

### Dataset Size

The workbook contains datasets ranging from 72 records to more than one million records.

The largest dataset is:

- geolocation_dataset

The central transactional dataset is:

- orders_dataset

---

### Missing Values

Missing values were identified primarily in the products dataset.

These missing values will be addressed during the Data Preparation phase.

---

### Duplicate Records

No significant duplicate records were identified in the business transaction tables.

Duplicate entries observed within the geolocation dataset are expected due to multiple geographic coordinates sharing the same ZIP code prefix.

---

### Data Types

Most columns were correctly interpreted by Pandas.

Datetime columns were successfully recognized.

Further validation will be performed during the cleaning phase.

---

### Initial Quality Issues

The following issues were identified:

- Missing values in product-related attributes.
- Product category translation sheet requires header validation.
- Geolocation dataset contains expected duplicate location mappings.

---

# Profiling Outcome

The assessment confirmed that the dataset is suitable for analysis.

The identified data quality issues are manageable and will be addressed during the Data Preparation phase.

---

# Next Phase

The next phase is:

## Phase 4 – Data Preparation

This phase includes:

### Data Cleaning

- Missing value treatment
- Data type validation
- Header correction
- Duplicate handling
- Data standardization

### Feature Engineering

- Delivery duration
- Delivery delay
- Order value
- Freight ratio
- Seller performance metrics
- Customer metrics
- Delivery efficiency metrics

The prepared datasets produced during this phase will be used for Exploratory Data Analysis, SQL analysis, and Power BI dashboard development.