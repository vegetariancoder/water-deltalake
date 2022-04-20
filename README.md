### What is a data lake

- A data lake is a central location that holds large amount of data in its raw format, unmodified state.
- We can store the data in its as it is form and we need to define any structure for that.
- We can run different types of analytics—from dashboards and visualizations to big data processing, real-time analytics, and machine learning to guide better decisions.

### What is a datawarehouse

- A data warehouse is a central repository of information that can be analyzed to make more informed decisions. 
- Data flows into a data warehouse from transactional systems, relational databases, and other sources, typically on a regular cadence. 
- Business analysts, data engineers, data scientists, and decision makers access the data through business intelligence (BI) tools, SQL clients, and other analytics applications.

|  | Data Lake  | Data Warehouse  |
| :---:   | :-: | :-: |
| Data Structure | Raw | Processed |
| Purpose of Data | Not yet determined | Currently in use |
| Users | Data Engineers, Data Scientist | Business professionals |
| Accessibility | Highly accessible and quick to update | More complicated and costly to make changes |


### What are the challenges with the Data Lake

1. Small file problems (we have to write the code by ourself).
2. Modification such as updates and deletes are painful (working on rows).
3. Time travel is not possible and is not integreated.( Rollback options or time travel options)
4. Replaying Data is not possible as well.
5. Dynamic schema validation is also not possible.
6. Schema evolution is not possible.


### Why Delta Lake
1. It supports **ACID Properties (Atomicity,Consistency, Integrity, Durability)** unlike traditional data lake.
2. It supports **Time Travel** and can also support roll bak options.
3. It can handle **upserts and deletes** and can also supports the **change data capturing (CDC)**.
4. It also supports **schema evolution and enforcement** . We can apply some constraints (means checks and filters).
5. It can handle both **streaming and batch** data.
6. It can handle the **scalable metadata** (can scale upto xetabytes)

