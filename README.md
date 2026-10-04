# Excel Badly Structured Data Transformation

## 📌 Project Overview

This project demonstrates an end-to-end **Excel data cleaning and transformation workflow** using **Microsoft Excel Power Query**.

The original dataset was highly disorganized, containing multi-level headers, sparse matrix structures, blank cells, and horizontally distributed data. The objective was to transform this structure into a standardized, analysis-ready tabular format.

## 🛠️ Tools & Technologies

* Microsoft Excel
* Power Query
* Data Cleaning
* Data Transformation
* Unpivoting
* Data Normalization
* Data Type Conversion

## 🎯 Problem Statement

The original Excel dataset contained several structural issues:

* Hierarchical multi-level column headers
* Ship Mode and Segment values distributed across multiple header levels
* Sales values scattered across a wide matrix
* Numerous blank cells
* Date information distributed across rows
* Data arranged horizontally instead of in a standard tabular structure

These structural issues made the dataset difficult to analyze, aggregate, and use for downstream reporting.

## 🔄 Transformation Process

The dataset was transformed using a reproducible Power Query workflow.

### 1. Table Transposition & Boundary Alignment

The initial cross-tabulated structure was transposed to flatten the hierarchical headers and align the attributes.

### 2. Fill Down

Null values created during the header restructuring process were filled down to preserve the correct grouping and context.

### 3. Unpivot Transformation

The wide matrix structure was converted into a normalized vertical format using **Unpivot Other Columns**.

This transformed the scattered Sales values into a structured attribute-value format.

### 4. Text Parsing & Date Extraction

Composite text and date-related information were extracted and converted into standardized data types.

### 5. Data Cleaning

Unnecessary text artifacts and empty cells were removed to prepare the resulting dataset for accurate calculations and analysis.

## 📊 Final Dataset Structure

The transformation produced a cleaner database-style structure containing fields such as:

| Field     | Data Type | Purpose                    |
| --------- | --------- | -------------------------- |
| Ship Mode | Text      | Distribution/shipping tier |
| Segment   | Text      | Customer classification    |
| Date      | Date      | Time dimension             |
| Sales     | Decimal   | Transactional sales metric |

## 📈 Business Value

The transformation provides a standardized dataset that can be used for:

* Data analysis
* Business intelligence dashboards
* Sales reporting
* Pivot-table analysis
* Database-oriented workflows
* Future Power Query refreshes

The Power Query approach also makes the transformation process reproducible, reducing the need for manual copy-paste operations.

## 🎓 Skills Demonstrated

* Excel Data Cleaning
* Power Query
* Data Transformation
* Unpivoting
* Data Normalization
* Data Preparation
* Handling Hierarchical Headers
* Date Extraction
* Structured Data Modeling
* Reproducible ETL Workflow
