🏡 Home Sales Analysis with SparkSQL

📘 Overview

This project showcases a comprehensive big data analysis of home sales using Apache Spark and SparkSQL. Leveraging PySpark, the analysis derives valuable insights from large-scale real estate transactions and demonstrates key performance optimizations through caching and partitioning. This work was completed as part of an academic capstone project and portfolio showcase.

🧰 Technologies Used

Python

Apache Spark (PySpark)

SparkSQL

Google Colab / Jupyter Notebook

AWS S3 (Cloud Data Storage)

📁 Dataset

The dataset is a revised real estate transaction file hosted on AWS S3:

home_sales_revised.csv

💡 Project Objectives

Load and process large datasets using Spark DataFrames

Perform analytical SQL queries on real estate features

Compare runtime performance using Spark caching and partitioning

Store and access partitioned data in efficient Parquet format

Demonstrate cloud-integrated data analysis using AWS S3

✅ Key Deliverables

Ingested and explored housing data via Spark DataFrames

Created a temporary SQL view from the dataset

Executed SparkSQL queries to extract:

Yearly average price of 4-bedroom homes

Year-built average price for 3-bed, 3-bath properties

Year-built average for 3-bed, 3-bath, 2-floor homes ≥ 2,000 sqft

Average price by "view" rating for homes priced ≥ $350,000

Cached the home_sales table to benchmark performance

Partitioned data by date_built and saved as Parquet

Validated cache/uncache operations

📊 Query Highlights

Average Price of 4-Bedroom Homes by Year

Year

Avg Price

2014

296,352.30

2015

298,859.45

Average Price by View Rating (≥ $350,000)

View

Avg Price

4

400,219.25

5

452,586.92

🚀 Performance Optimization

Caching: Cached the SQL view to reduce recomputation and boost performance on repeated queries.

Partitioning: Used column-based partitioning (date_built) and Parquet format to optimize query efficiency and data handling.

☁️ Cloud Integration

This project demonstrates remote data integration by accessing datasets stored in Amazon S3, simulating real-world cloud analytics workflows.

🕒 Runtime Comparison

Query Type

Runtime (seconds)

Uncached

~2.1s

Cached

~0.5s

Parquet

~0.6s

🚀 How to Run This Project

Clone this repository:

git clone https://github.com/yourusername/Home_Sales.git

Open Home_Sales.ipynb in Google Colab or Jupyter Notebook

Execute all code cells sequentially to reproduce the analysis



