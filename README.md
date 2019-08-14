# Data Warehouse: Using Redshift and S3
> Anita Quevedo Solidoro

This ETL Pipeline was designed for a startup **Sparkify**, who wants to analyze their information collected about the songs and the activity of their users in their new music streaming application, this project creates a star-schema database using Amazon Redshift from a directory in S3 of JSON metadata of songs and the activity on the apps.

### Files in Project
The main files  for running the project are:

* `InfrastructurE_Code.py`: to create data warehouse on Amazon Redshift using IAM Role for s3 access, the method is the creation infrastructure with code(python)

* `dwh.cfg`: the archive has configuration Redshfit and S3.

* `create_tables.py`: Script drop tables if exist, to create and modify relations that between.

* `sql_queries.py`: Script with the queries and scripts to use in create_tables.py and etl.py.

* `etl.py`: connects to Redshift and ingest data from S3 and insert data into fact and dimensional in the tables that were created.




### How to run in the console: 

1) Deploy a data warehouse on Amazon Redshift using IAM Role for S3 access.
2) Configure dwh.cfg with credentials and information of your Redshift coneection and s3 roots.
3) Run in the console python create_tables.py
4) Run in the console pyhton etl.py

And later, you you will be able to visualize the tables created in the redshift console of the amazon page in the query editor tab:
https://prnt.sc/o1wfdz

## Recommendation ---> do not forget to remove the machine if you do not use it


