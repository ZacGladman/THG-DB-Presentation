* Originally given MLDB 
* some stuff on this 
* image
***
![BigQuery And Its Amazing Features(Try BigQuery for free) | Medium](https://miro.medium.com/v2/resize:fit:878/1*jNf8QbZbZ2L56A4a8UKWHQ.png)
***
## History & Background

Launched in 2011 it is a fully managed serverless data warehouse that enables scalable analysis of petabytes of data. 
* it is an example of PaaS and uses a dialect of SQL
* A big feature of BigQuery is its built in machine learning techology
* BigQuery provides external access to Google's Dremel technology
***
## Design and architecture
![https://storage.googleapis.com/gweb-cloudblog-publish/images/BQ_Explained_2.max-900x900.jpg](https://storage.googleapis.com/gweb-cloudblog-publish/images/BQ_Explained_2.max-900x900.jpg)

***
## Dremel

***
## Where does it fall in the CAP model, Why?
![CAP Theorem 23 Years Later with Eric Brewer - Software Engineering Daily](https://i0.wp.com/softwareengineeringdaily.com/wp-content/uploads/2023/05/cap.png?resize=730%2C389&ssl=1)

* #### Generally used for analytics
* #### Not being used for CRUD operations on a production application

***
## Pros and Cons

### Pros:

- good for very large datasets (petabyte-sized) (maybe a waste if they're not that big).
- great at complex queries (again, a waste if you're just running simple SELECT statements).
- is a serverless, making it good in high-concurrency scenarios; some BigQuery users have claimed to run up to 10,000 queries at once.
- offers in-built machine learning features; don't need to write own algorithms in Python or Java.
- uses familiar SQL syntax.
- no need to move data from the data warehouse to elsewhere, e.g. external Python-based ML frameworks; it brings ML to the data.
- this increases speed of development/innovation.
- can process trillions of rows per second.

***
## Pros and Cons
### Cons:

- should not be used to substitute a relational database; it is oriented on running analytical queries, not CRUD operations.
- not great a join operations.
- it is a paid service; you pay based on how big your query is, so you must make them as efficient as possible.
- dependent on the Google Cloud Platform; need to be comfortable using it.
- potentially steep learning-curve in terms of data warehousing.
- might not be easy to integrate with non-GCP tools.

***
## Describe some use cases of the database
## Use Cases

- great for analysing huge sets of historical data/data that doesn't change much.
- in-built ML is good for things like anomaly detection (useful for identifying credit card fraud), customer segmentation (k-means clustering) or sales forecasting.
***
