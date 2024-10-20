# HHA504_assignment_dbs

# Working with Managed Databases in Azure and GCP

## Overview
In this project, I got to work with both Azure and Google Cloud Platform (GCP) to manage databases. The main tasks were:
- Setting up MySQL databases in both Azure and GCP.
- Querying a dataset using BigQuery on GCP.
- Monitoring database performance on both platforms.
- Comparing the experience of using managed databases on Azure and GCP.

---

## 1. Database Creation and Setup

### Azure MySQL
For Azure, I created an **Azure Database for MySQL** instance.

![Screenshot 2024-10-17 154721](https://github.com/user-attachments/assets/55936759-36e2-432c-99c1-f33cbdcdc8f5)


### GCP MySQL (Cloud SQL)
I also set up a MySQL instance on **Cloud SQL** in GCP. 

![Screenshot 2024-10-17 165354](https://github.com/user-attachments/assets/72fc5064-12c4-4238-b934-26efb357cf5e)


---

## 2. BigQuery Exploration

### Uploading Data to BigQuery
I uploaded the **TOP 100 IMDB MOVIES.csv** file into the dataset I created on BigQuery, which is called `imdb_movies`. 

![Screenshot 2024-10-17 171007](https://github.com/user-attachments/assets/1407681d-5fb6-44bc-b6fa-9c6d5975e414)


### Running a Query in BigQuery
Once the data was uploaded, I ran a SQL query to get the movies with a rating of 9.0 or higher.

**SQL Query:**
```sql
SELECT title, year, rating
FROM `shveta-sharma-hha504.movies.imdb_movies`
WHERE rating >= 9.0
ORDER BY rating DESC;
```

# Reflections on Managing Databases on Azure vs. GCP

### Azure MySQL
Azure's MySQL setup was straightforward and easy to follow. The monitoring tools were detailed, which helped me keep track of the database’s performance. I found the interface user-friendly as well.

### GCP MySQL
GCP's Cloud SQL was also easy to set up. GCP stands out with **BigQuery**—it made handling large datasets faster and more efficient.

# Monitor Database Services

## Azure MySQL Monitoring
In Azure, I used the portal to monitor the performance and cost of the MySQL database. I explored key metrics such as:
- **CPU Usage**: I checked how much of the server's processing power was being used.
- **Memory Usage**: I monitored the memory consumption of the MySQL database.
- **Query Performance**: I tracked the execution time of queries and overall database responsiveness.


## GCP MySQL and BigQuery Monitoring
In GCP, I monitored both the Cloud SQL MySQL instance and the BigQuery dataset. Similar to Azure, I explored:
- **CPU Usage**: GCP provided insights into how much CPU power was being utilized by the Cloud SQL instance.
- **Memory and Disk I/O**: I checked memory and disk input/output operations for the Cloud SQL instance.
- **BigQuery Performance**: I also monitored the costs and performance of running queries in BigQuery, focusing on query execution time and cost.


---

## Differences in Monitoring Tools Between Azure and GCP
- **Azure**: The monitoring dashboard was very detailed, especially for MySQL. It provided real-time insights into resource usage and query performance, making it easier to monitor the database performance.
- **GCP**: GCP’s monitoring for Cloud SQL was less detailed than Azure's, it still offered key metrics like CPU, memory, and disk usage. **BigQuery** monitoring stood out for tracking query performance and costs effectively, especially for large datasets.





---

