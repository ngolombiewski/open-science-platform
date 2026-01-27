# OpenAlex Research Data Platform

Work in progress – building a production-style data pipeline for global research metadata using OpenAlex and a modern data stack.
This is meant to become a capstone project for the Data Engineering Zoomcamp 2026.

---

## Problem Idea (draft)

Research metadata is highly relational, deeply nested, and continuously evolving.  
Publications link to authors, institutions, concepts, and citations, forming a complex graph of relationships.

This project aims to build a data pipeline that:

1. Ingests research metadata from the OpenAlex API in batches
2. Stores raw data in a cloud data lake
3. Processes and normalizes the data into a structured form
4. Loads it into a data warehouse optimized for analytics
5. Transforms the data into analytical models using dbt
6. Serves the data through a simple dashboard


---

## High-Level Architecture (draft)

OpenAlex API  
- Batch ingestion
- Raw JSON in Data Lake  
- Processing / normalization  
- Structured staging data  
- BigQuery Data Warehouse  
- dbt transformations  
- Dashboard

---

## Planned Technology Stack

- Cloud: GCP
- Infrastructure as Code: Terraform
- Orchestration: Dagster
- Data Lake: GCS
- Processing: to be decided
- Data Warehouse: BigQuery
- Transformations: dbt
- Dashboard: Looker Studio or Streamlit

The exact processing engine between raw lake data and the warehouse is intentionally left open for now.

---

## Data Source

OpenAlex (https://openalex.org/) is an open catalog of scholarly works, authors, institutions, and concepts.
