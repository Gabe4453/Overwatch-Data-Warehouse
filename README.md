# Overwatch Analytics Warehouse

A data engineering portfolio project that extracts live Overwatch player statistics from the OverFast API, stores them in SQL Server, and models the data using a dimensional warehouse design.

## Project Goal

The goal of this project is to build an end-to-end ETL pipeline that tracks Overwatch player performance over time.

## Tech Stack

- Python
- SQL Server
- pyodbc
- OverFast API
- GitHub
- Power BI

## Architecture

OverFast API  
↓  
Python ETL Pipeline  
↓  
JSON Staging Files  
↓  
SQL Server Data Warehouse  
↓  
Power BI Dashboard

## Data Warehouse Tables

### Dimension Tables

- DimPlayer
- DimHero
- DimRole
- DimDate

### Fact Tables

- FactHeroStats
- FactRoleStats

## Current Features

- Extracts live player profile data
- Extracts hero performance stats
- Extracts role performance stats
- Loads data into SQL Server
- Prevents duplicate daily snapshots
- Tracks historical player performance over time

## How to Run

```bash
python etl/run_pipeline.py
