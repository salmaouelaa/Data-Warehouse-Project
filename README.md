# Data Warehouse & Analytics Project

**End-to-End Data Engineering | SQL Server | ETL Pipelines | Dimensional Modeling | SQL Analytics**

## Overview

Designed and implemented an end-to-end SQL Data Warehouse that integrates CRM and ERP data into a centralized, analytics-ready platform.

The project demonstrates the complete data engineering lifecycle, from raw data ingestion and transformation to dimensional modeling and business reporting, following modern data warehousing practices.

## Business Problem

Organizations often store customer, product, and sales information across disconnected operational systems. Differences in data formats, inconsistent records, and fragmented data structures make it difficult to produce reliable business reports.

**The objective:** Build a unified, reliable source of analytical data that supports sales performance monitoring, customer analysis, and data-driven decision-making.

## Solution & Architecture

Implemented a **Medallion Architecture** with three layers to separate ingestion, data quality, and analytical consumption.

| Layer      | Responsibility                                                                     |
| ---------- | ---------------------------------------------------------------------------------- |
| **Bronze** | Ingest raw CRM and ERP datasets while preserving source data.                      |
| **Silver** | Clean, standardize, validate, and prepare data for integration.                    |
| **Gold**   | Deliver business-ready fact and dimension tables optimized for analytical queries. |

### Key Engineering Components

- **ETL Pipelines:** Developed SQL-based batch pipelines using stored procedures to automate ingestion and transformation across warehouse layers.
- **Data Quality & Integration:** Applied deduplication, null handling, data standardization, and business-rule validation to reconcile data from multiple source systems.
- **Dimensional Modeling:** Designed a Star Schema with customer and product dimensions and a sales fact table to simplify analytical queries.
- **Analytics & Reporting:** Developed SQL-based analytical queries to support revenue analysis, product performance evaluation, and customer insights.

## Data Model

The Gold layer follows a **Star Schema**, separating measurable business events from descriptive dimensions.

This design enables efficient aggregation, filtering, and reporting while providing a structured foundation for downstream BI applications.

## Business Value

The resulting warehouse provides:

- **Unified data:** Consolidated customer, product, and sales information from CRM and ERP systems.
- **Improved data reliability:** Standardized records and consistent business rules.
- **Analytics-ready structure:** Reusable fact and dimension tables for reporting.
- **Business visibility:** A foundation for analyzing revenue, sales trends, product performance, and customer behavior.

## Skills Demonstrated

`SQL Development` · `Data Architecture` · `Data Engineering` · `ETL Pipeline Development` · `Data Integration` · `Data Quality` · `Dimensional Modeling` · `Data Analytics`

## Project Documentation

- [Data Catalog](docs/data_catalog.md)
- [Star Schema Diagram](docs/data_model_star_schema.png)
- [Gold Layer SQL](scripts/gold/ddl_gold.sql)

## Future Enhancements

- Implement incremental data loading and pipeline orchestration.
- Extend automated data quality and integrity testing.
- Develop Power BI dashboards for interactive business reporting.

---

**Project Focus:** Building a reliable analytical data foundation through structured data engineering, scalable modeling practices, and SQL-based analytics.
