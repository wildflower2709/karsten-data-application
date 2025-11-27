Python ETL Pipeline (Extract-Transform-Load)

Status: Completed / In Progress
Tools: Python, Pandas, SQLAlchemy, SQLite / Azure SQL, Requests

📌 Project Overview

This project showcases my ability to build automated ETL pipelines using Python.
It extracts data from a CSV file or API, cleans & transforms it using pandas, and loads it into a SQL database.

This demonstrates data engineering fundamentals relevant to roles requiring ETL/ELT workflow creation.

🎯 Objectives

Write Python scripts to extract and clean raw data

Remove duplicates, handle missing values, format columns

Load the cleaned dataset into a SQL database (SQLite or Azure SQL)

Log key steps & errors

Prepare the pipeline for integration with cloud tools

⚙️ Tools & Libraries
import pandas as pd
import requests
from sqlalchemy import create_engine
import logging

📂 Pipeline Steps
1. Extract

Input: CSV file and/or REST API

API fetched using Python requests

2. Transform

Data cleaning (missing values, type conversions)

Feature engineering

Standardized column names

3. Load

Load into sqlite (database.db)

OR Azure SQL using SQLAlchemy engine

🧪 Example Code Snippet
df = pd.read_csv("sales.csv")

df.drop_duplicates(inplace=True)
df['Date'] = pd.to_datetime(df['Date'])

engine = create_engine("sqlite:///database.db")
df.to_sql("SalesCleaned", engine, if_exists="replace", index=False)

📁 Files Included

etl_pipeline.py

requirements.txt

Sample dataset

database.db (output)

Log file

📥 How to Run
pip install -r requirements.txt
python etl_pipeline.py

▶️ Optional Enhancements

Run pipeline daily using cron / Task Scheduler

Connect Python pipeline to Azure Data Factory

Add unit tests

Add cloud storage integration

Add Power BI README.
