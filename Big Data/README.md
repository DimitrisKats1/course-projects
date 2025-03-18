# Large-Scale Data Processing with Apache Spark & Hadoop

This project demonstrates processing and analyzing large-scale crime data from Los Angeles using distributed computing frameworks, specifically **Apache Spark** and **Hadoop (HDFS)**.

## Tools and Technologies:
- Apache Spark (v3.4+)
- Apache Hadoop (v3.0+)
- Spark DataFrame, SQL, and RDD APIs

## Datasets:
- **Primary Dataset**: [Los Angeles Crime Data (2010 - present)](https://data.lacity.org/)
- **Secondary Datasets**:
  - [LA Police Stations](https://geohub.lacity.org/datasets/lahub::lapd-police-stations/explore)
  - [Median Household Income by Zip Code (2015)](http://www.laalmanac.com/employment/em12c_2015.php)
  - Reverse Geocoding data provided for mapping coordinates to ZIP Codes.

## Analysis Performed:
- **Query 1**: Identified top 3 months per year with highest crime incidents.
  - Compared performance using CSV and Parquet formats, and SQL vs DataFrame APIs.

- **Query 2**: Analyzed and ranked times of day (Morning, Afternoon, Evening, Night) based on street crimes.
  - Implemented using DataFrame/SQL and RDD APIs.

- **Query 3**: Investigated victim demographics (descent) in ZIP Codes with highest and lowest median household incomes.
  - Tested and compared various Spark join strategies (`BROADCAST`, `MERGE`, `SHUFFLE_HASH`, `SHUFFLE_REPLICATE_NL`) and evaluated their performance.

- **Query 4**: Calculated incidents involving firearms per police precinct and average distances to each precinct.
  - Implemented custom broadcast and repartition joins using the RDD API.
  - Performed the same analysis using DataFrame API.

## Key Takeaways:
- Apache Parquet format significantly improved query performance compared to CSV.
- DataFrame and SQL APIs typically offered superior performance and ease-of-use compared to RDDs.
- Optimizing join strategies based on dataset characteristics notably enhanced query efficiency.

## Setup and Environment:
- Deployed a fully distributed Hadoop and Spark environment with multiple nodes.
- Stored datasets on Hadoop Distributed File System (HDFS).

