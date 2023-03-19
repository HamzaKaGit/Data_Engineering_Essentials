
# Top Data Terms You Should Know

In today's `data-driven` world, data is an essential part of every business `decision-making process.` However, with the vast amount of data available, it can be difficult to understand the different terms and concepts. From Big Data to Data Lake, Database to Data Warehouse, understanding these terms and how they relate to each other is crucial in `unlocking the value of data.` 
## What is Data?
Data is a collection of `facts,` `figures,` and `statistics` that are raw, unorganized, and unrelated pieces of information. It can be in various forms such as numbers, text, images, videos, and sound.

Data is generated from various sources, including `human-generated` data such as surveys, social media posts, and medical records, and `machine-generated` data such as sensor readings, GPS signals, and financial transactions.

## Types of Data:

Data can be categorized into `three types` based on their properties:
- Structured.
- Unstructured.
- Semi-Structured.

### Structured data:
It is `highly organized` and `formatted` in a `specific way` that makes it easy to `process and analyze.` Examples of structured data include data stored in `databases` or `spreadsheets` that allow for efficient `storage and querying` of data.

### Unstructured data:
on the other hand, Unstructured Data `lacks` a specific format or structure. This makes it `difficult to analyze` and process with `traditional data processing tools.` Examples of unstructured data include `emails,` social media posts, and audio/video recordings.

### Semi-structured data:
It is data that has some structure but is not as `organized as structured data.` Semi-structured data may contain `tags,` metadata, or other markers that help to organize and structure the data. Examples of semi-structured data include `XML or JSON files.`









## Database:
A database is a `structured collection` of data that is organized in a `specific format` and can be: 
- Accessed
- Managed 
- Updated 
by authorized users. 

#### It is designed to:
- Store
 - Retrieve
 - Manage 
 structured data that is related to a `specific domain` or `application.`

## Types of Databases:
There are several types of databases, each with its unique `features and advantages.` Here are some of the most common types of databases along with their descriptions:

### Relational Database:
 A relational database is a type of database that organizes data into `one or more tables,` with a `unique key` identifying each row. It uses `SQL (Structured Query Language)` for `managing` and `manipulating data.`

### NoSQL Database:
A NoSQL database is a non-relational database that uses a `flexible schema` to store data. It is designed to handle `unstructured,` `semi-structured,` and `highly variable` data types. NoSQL databases are highly scalable and can handle `large volumes of data,` making them ideal for `big data applications.`

## Data Warehouse:
A data warehouse is a `central repository` that stores data from `multiple sources` in a `structured format,` making it easier to analyze and derive insights. It is designed to support business intelligence (BI) activities such as `data mining`, `reporting,` and `decision-making` by providing a consolidated view of the organization's data.

## Data Lake:
A data lake is a `centralized repository` that stores `raw,` `unprocessed,` and `unstructured data` at scale. It is designed to store data in its native format, and can handle large volumes of data from diverse sources such as social media, web logs, and IoT devices. A data lake is used to store `all types` of data, including structured, semi-structured, and unstructured data, making it a highly flexible and scalable storage solution.

## Big Data:
Refers to the `massive volume` of `structured,` `semi-structured,` and `unstructured data` that is generated from various sources at high velocity and in real-time. It is characterized by the 3Vs `(Volume, Velocity, and Variety),` and often requires `specialized tools` and `technologies to process,` `analyze,` and `derive insights` from it.

## Real-World Scenario:
Suppose a company collects data from various sources such as `social media,` `customer interactions,` and `sales transactions.` This data is stored in a data lake in its `raw and unprocessed form.` The company then uses `big data tools` and `technologies` to `process` and `analyze this data,` which helps them to gain valuable insights about customer behavior, market trends, and other important metrics.

The `insights` derived from the `data lake` are then stored in a `data warehouse,` which provides a `consolidated view` of the company's data, making it easier to analyze and derive insights. The data warehouse is designed to support business intelligence activities such as `reporting and decision-making.`

The data in the data warehouse is organized in a `structured format,` which makes it easier for authorized users to `access,` `manage,` and `update` the data. This data can also be used to `build applications` such as `dashboards and reports,` which provide `real-time insights` to `decision-makers.`


## Data Marts:
Data marts are smaller `subsets` of a larger `data warehouse` that are designed to serve a `particular` business function or department. They contain a `specific set` of data that is `relevant` to a particular group of users.

## Data Lakehouse: 
A data lakehouse is a data `storage and management system` that `combines` the best features of `data lakes` and `data warehouses.` It provides a `unified architecture` for `storing,` `managing,` and `analyzing data` in real-time.

## Data Mesh: 
Data mesh is a `new architectural approach` to `managing data` in a large organization. It emphasizes `decentralized data ownership and management,` and it seeks to create a `data infrastructure` that is both `scalable` and `flexible.`

## OLTP vs OLAP:
Online Transaction Processing and Online Analytical Processing are two different approaches to `managing and analyzing data.` OLTP is designed for `processing` and `managing transactions` in `real-time,` such as sales transactions or financial transactions. OLAP, on the other hand, is designed for analyzing `large sets of data,` such as `customer data` or `product data.`

## Real world scenario:
Consider a large `retail organization` that operates in multiple countries and has millions of customers. The organization collects data from various sources, including `point of sale systems,` `online transactions,` `social media,` and `customer feedback.` This data is stored in a `data lake,` which serves as a `central repository` for all the `raw data.`

To make sense of this data, the organization uses a `combination` of `data marts` and `OLAP`. Each data mart is designed to serve a `particular business function,` such as `sales or marketing.` The data in each data mart is organized in a specific way, and it is optimized for `querying and analysis.`

The OLAP system is used to `analyze the data` in the `data marts` and to `generate reports and dashboards.` This allows the organization to gain `insights` into customer behavior, sales trends, and marketing effectiveness.

Finally, the data mesh approach is used to ensure that the `data infrastructure` is `scalable and flexible.` Each `business unit` is responsible for managing its own data, and the organization uses a `decentralized approach` to `data management.` This allows the organization to `quickly adapt` to `changing business needs` and to `scale its data infrastructure` as needed.
