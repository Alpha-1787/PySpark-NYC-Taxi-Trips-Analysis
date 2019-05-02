# Overview
Here I am exploring a public data set that Google BigQuery has provided us. In particular we will be looking at the 2018 Yellow Taxi trips and the weather data set together. 

Throughout the work, I have consciously chosen to work with dataframes and the dataframe API in Spark Mllib (commonly referred to as Spark ML) over working with hand-coded implementations with RDDs. Typically, using RDDs coded in Python would allow greater flexibility, but at the cost of serialization/deserialization of the data and code to something Spark can understand. In addition I also consciously try to avoid using User defined functions (UDFs) suffer from the same setback to avoid the performance loss due to serialization/deserialization that occurs. Instead, I try to take advantage of the dataframe api and all the optimizations that comes with it.

 Please note that without modifications the notebook  can only be run no a cluster, and not locally on a python 3 kernel.

