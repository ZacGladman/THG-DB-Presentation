## Pros and Cons

### Pros:

- good for very large datasets (petabyte-sized) (maybe a waste if they're not that big).
- great at complex queries (again, a waste if you're just running simple SELECT statements).
- is a serverless, making it good in high-concurrency scenarios; some BigQuery users have claimed to run up to 10,000 queries at once.
- offers in-built machine learning features; don't need to write own algorithms in Python or Java.
- uses familiar SQL syntax.
- super-fast SQL queries using the processing power of Google’s infrastructure.
- can process trillions of rows per second.



### Cons:

- should not be used to substitute a relational database; it is oriented on running analytical queries, not CRUD operations.
- not great a join operations.
- it is a paid service; you pay based on how big your query is, so you must make them as efficient as possible.
- dependent on the Google Cloud Platform; need to be comfortable using it.
- potentially steep learning-curve in terms of data warehousing.
- might not be easy to integrate with non-GCP tools.


## Use Cases


