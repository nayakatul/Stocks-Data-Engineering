# Stocks Near-Real-Time Data Analysis and Visualization Project


**Overview**

In this project, I am running ETL pipelines using Apache Airflow to collect (6 years of historical + near real-time) stock data from the Alpaca API, process it, and store it in two Google BigQuery tables:

-	Table 1: Stores 1-day interval stock data (One-time ETL run + incremental ETL runs daily).
-	Table 2: Stores 5-minute interval stock data (One-time ETL run + incremental ETL runs every 10 minutes).

I am using Google Cloud Engine to run Airflow in a Docker container spun up using a docker-compose file. I have connected Looker Studio to the BigQuery tables and SQL views to create different visualizations for analyzing stocks.

**Architecture and Data Flow**

![alt text](https://github.com/nayakatul/Stocks-Data-Engineering/blob/main/Stocks_data_Arch-Diagram.png)


