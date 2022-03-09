# ETL Pipeline for Immigration, Airports, and Cities Data
### Data Engineering Capstone Project

#### Project Summary

The goal of this project is to pull and combine disparate datasets that together would offer multifaceted responses to the business user who may be interested in learning more about the US travel and immigration/travel event correlation. I will be creating an ETL pipeline using publicly available immigration data and city/airport data that would allow me to create a database that is optimized for queries on travel events. 

Since this data provides insights only once accumulated, I would recommend setting up an Airflow refresh no more frequent than once per quarter.

The reason I would recommend using Aiflow is for its simplicity of use, transparency that it brings to the ETL process, and free license. For data processing, I stuck to Pandas and PySql as those are straightforward tools I'm very familiar with. They do the job, and do it well.

The project (**etl.ipynb**) follows the below steps:
* [Step 1: Scope the Project and Gather Data]
* [Step 2: Explore and Assess the Data]
* [Step 3: Define the Data Model]
* [Step 4: Run ETL to Model the Data]
* [Step 5: Complete Project Write Up]

The following tables are created:
* FACT Table with Immigration events
* DIM Table with Airport attributes
* DIM Table with City attributes

Tables are optimized to facilitate queries, such as:
* Is there a correlation between the volume of travel and the number of entry ports?
* Does the volume of travel depend of the demographics of a given city?
* Which visa type holders comprise the majority of travelers in a given airport / city?

Libraries:
* pandas
* numpy 
* pyspark.sql
* pyspark.sql.functions
