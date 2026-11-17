# SWYNEX-Data-Preparation

📊 SWYNEX: Data Preparation & Cleaning

📌 Project Overview

Before diving into Power BI for interactive dashboarding and business intelligence, raw retail data requires a thorough quality check to ensure the final visuals tell an accurate story. This repository documents the data preparation, sanitization, and validation workflow performed on the Sample Superstore dataset to make it ready for downstream data modeling.

🗂️ Dataset Information

Source: Sample Superstore Dataset (Kaggle)

Domain: Retail & E-Commerce

Contents: Core retail transaction records covering customer demographics, order timelines, shipping modes, regional performance, revenue (Sales), and Profit margins.

🧹 Data Cleaning & Transformation Workflow

To guarantee data integrity and prevent calculation errors in Power BI, the following three-step cleaning pipeline was executed in Excel:

Deduplicated Records

Scanned the entire dataset and stripped out exact duplicate rows using Excel's Remove Duplicates utility so that total sales figures and order counts are not artificially inflated.

Verified Nulls & Missing Values

Audited column filters across all categorical and dimensional fields to confirm zero blank cells, nulls, or corrupted text entries that could break dashboard slicers or visual filters.

Standardized Data Types

Enforced strict schema formatting across all fields:

Text/Categorical: Ship Mode, Customer Name, Segment, Region, etc.

Numeric/Currency: Sales, Quantity, Discount, and Profit formatted strictly as numbers for accurate DAX aggregations.

📁 Repository Structure

SWYNEX-Data-Preparation/
├── data/
│   └── Cleaned_Superstore.csv    # Sanitized, analysis-ready dataset
└── README.md                     # Project documentation


🚀 Final Output & Next Steps

Deliverable: The polished, analysis-ready dataset is saved as Cleaned_Superstore.csv.

