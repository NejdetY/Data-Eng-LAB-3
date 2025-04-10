# Data-Eng-LAB-3
Transforming Data Using a Serverless SQL Pool in Azure Synapse Analytics
Project Summary
The main goal was to process and transform raw, semi-structured data stored in Azure Data Lake Storage.
Using serverless SQL, I queried and cleaned the data, performed aggregations, and stored the results in a
more optimized format for further analysis. All operations were executed through Synapse Studio, which
provides a code-first, browser-based environment for data professionals.
Key Steps Performed
1. Environment Setup:
- Created an Azure Synapse workspace.
- Configured Azure Data Lake Storage Gen2 and linked it to the Synapse workspace as the default storage.
2. Uploading Raw Data:
- Uploaded a sample dataset in CSV format to a specific container in the data lake.
3. Querying Raw Files:
- Used the OPENROWSET function in serverless SQL to query the CSV files directly.
- Selected only the necessary columns to improve performance and reduce noise in the dataset.
4. Data Transformation and Aggregation:
- Aggregated total sales per product per year using standard SQL.
- Saved the result set into an external table in Parquet format using the CREATE EXTERNAL TABLE AS
SELECT (CETAS) command.
Transforming Data Using a Serverless SQL Pool in Azure Synapse Analytics
5. Automating with Stored Procedures:
- Created a stored procedure to automate the data transformation process.
- This procedure can be executed at any time to reprocess and refresh the aggregated data.
Skills and Concepts Learned
- Setting up and using Azure Synapse Analytics and serverless SQL pools
- Reading raw data files from a data lake using SQL
- Data transformation, filtering, and aggregation in SQL
- Writing optimized Parquet output using external tables
- Automating ETL workflows using stored procedures
Conclusion
This hands-on project provided valuable experience in working with cloud-native data engineering tools. The
serverless SQL pool feature proved to be a flexible and cost-effective solution for querying and transforming
large datasets without the need for dedicated infrastructure. This method is especially useful for teams
looking to build scalable, on-demand data pipelines in Azure.
