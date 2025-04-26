
## Problem Overview

Real-world data isn't always in structured format — it’s messy, scattered, and mostly unstructured.
In this project, I challenged myself to take unstructured Twitter data and transform it into a structured, analytical-friendly format.

## Tools and Technologies

- PySpark: For distributed processing and handling semi-structured data.

- MongoDB: To store the raw unstructured tweets (because relational databases aren't fit for semi-structured data).

- SQL (via SparkSQL): To query and organize the data after structuring.
# Project Workflow
- **Data Storage**:
Tweets were stored in MongoDB under the "Tweets" database.

- **Data Ingestion**:
Established a connection between PySpark and MongoDB. Loaded the data into PySpark using spark

- **Understanding the Raw Structure**:
Inspected the schema to identify nested fields and arrays and used explode() to flatten nested lists and fields then created a temporary view (myTweet) to run SQL queries over the data.

- **Data Aggregation**:
Grouped tweets by user and creation time and computed:

- **Final Output**:

Achieved a clean, fully structured dataset ready for deeper analysis or modeling.

![image](https://github.com/user-attachments/assets/ffae9fb0-e08d-45e3-a667-2c4f0f39300a)




## Conclusion
- Learned to handle and process semi-structured data (one of the most crucial real-world data challenges).

- Strengthened my ability to connect PySpark with NoSQL databases like MongoDB.

- Gained hands-on practice exploding and flattening complex nested fields.

- Developed a smooth SQL-on-Spark querying workflow for large datasets.
