# Home_Sales
Homework for Module 22 - Big Data


This project is an exercise in using Spark to perform data analysis based on a csv file hosted in an Amazon S3 bucket.

Once the file is loaded, the csv is read into a DataFrame which is then converted to a temporary view to perform SQL queries against.

Several Spark SQL queries are performed against the initial view, then once again on the view after it has been cached.

Lastly, we load the dataframe into parquet files partitioned by date_built and perform another sql query against a view created from the partitioned parquet files.

Query run times are tracked to indicate how caching and partitioning the data impacts performance.

**Note:** This notebook is designed to run in a Google Colab environment.