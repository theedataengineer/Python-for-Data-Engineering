### What is Data Engineering

#### Topics:

- What data engineers do
- Data engineering versus data science
- Data engineering tools

##### What Data Engineers Do

- The roles and responsibilties of a data engineer vary depending on an organization's level of data maturity and staffing levels.
- However, there are some tasks, such as the extracting, loading, and transforming of data, that are foundational to the role of a data engineer.

- Data Engineers - Query data from a source (extract), they perform some modifications to the data (transform, and then they put that data in a location where users can access it and know that it is production quality (load).

- ETL - Extract, Transform, Load


##### Example:

- An online retailer has a website where you can purchase widgets in a variety of colors. The website is backed by a relational database. Every transaction is stored in the database.

- Quiz: How many blue widgets did the retailer sell in the last quarter?

- Solution: You could run a SQL Query on the database.This doesnt reach to the level of needing a data engineer.

- BUT:
As the site grows, running queries on the production database is no longer practical. Furthermore, there may be more than one database tht records transactions.

i.e There may be a database at different geographical locations - for example, the retailers in North America may have a different database than retailers in Asia, Africa and Europe.

Now, you have entered the realm of data engineering.

- Solution: To answer the preceding question, a data engineer would create connections to all of the transactional databases for each region, extract the data, and load it into a data warehouse.

From there, you could now count the number of all the blue widgets sold.


###### New set of questions to ask

- How do we find out which locations sell the most widgets?
- How do we find out the peak times for selling widgets?
- How many users put widgets in their carts and remove them later?
- How do we find out the combination of widgets that are sold together?

###### NOTE:

- There is a transformation required in between the extract and load.
- There is also the differences in time zones in different regions.
- For instance: The United States alone has four time zones.


- Here, the data engineer would need to extract the data from each database, then transform the data by adding an additional field for the location.
- To compare the time zones, the data engineer would need to be famiiar with data standards.
- For the time, the International Organization for Standardization (ISO) has a standard - ISO 8601

- Revised Questions:

- 1. Extract the data from each database.
- 2. Add a field to tag the location for each transaction in the data.
- 3. Transform the date from local time to ISO 8601.
- 4. Load the data into the data warehouse.

Now, the combination of extracting, loading, and transforming data is accomplished by the creation of a data pipeline.

- The data comes into the pipeline raw, or dirty in the sense that there may be missing data or typos in the data, which is then cleaned as it flows through the pipe.
- After that, it comes out the other side into a data warehouse, where it can be queried.



```mermaid
graph TD;
	'Source data'-->Extract;
	Extract-->'Add location';
	'Add location'-->'Transform date';
	'Transform date'-->Load;
	Load-->'Clean data';
```
