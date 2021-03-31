# Mongo and Mongoose


copied from 
https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/

General Notes on NoSQL Data Modeling
The rest of this article describes concrete data modeling techniques and patterns. As a preface, I would like to provide a few general notes on NoSQL data modeling:

NoSQL data modeling often starts from the application-specific queries as opposed to relational modeling:
Relational modeling is typically driven by the structure of available data. The main design theme is  “What answers do I have?” 
NoSQL data modeling is typically driven by application-specific access patterns, i.e. the types of queries to be supported. The main design theme is “What questions do I have?”  
NoSQL data modeling often requires a deeper understanding of data structures and algorithms than relational database modeling does. In this article I describe several well-known data structures that are not specific for NoSQL, but are very useful in practical NoSQL modeling.
Data duplication and denormalization are first-class citizens.
Relational databases are not very convenient for hierarchical or graph-like data modeling and processing. Graph databases are obviously a perfect solution for this area, but actually most of NoSQL solutions are surprisingly strong for such problems. That is why the current article devotes a separate section to hierarchical data modeling.
Although data modeling techniques are basically implementation agnostic, this is a list of the particular systems that I had in mind while working on this article:
Key-Value Stores: Oracle Coherence, Redis, Kyoto Cabinet
BigTable-style Databases: Apache HBase, Apache Cassandra
Document Databases: MongoDB, CouchDB
Full Text Search Engines: Apache Lucene, Apache Solr
Graph Databases: neo4j, FlockDB

[<== Back](README.md)