---
title: Azure Synapse Link for Azure Cosmos DB Gremlin API supported features
description: Understand the features/restrictions using Azure Synapse Link for Azure Cosmos DB Gremlin API
services: synapse-analytics cosmosdb 
author: sesmyrnov
ms.service: synapse-analytics cosmosdb
ms.topic: conceptual
ms.subservice: synapse-link cosmosdb-graph
ms.date: 02/14/2022
ms.author: sesmyrno
ms.reviewer: mansha
ms.custom: cosmos-db
---

# Azure Synapse Link for Azure Cosmos DB Gremlin API - supported features

This article describes the functionalities that are currently supported in Azure Synapse Link for Azure Cosmos DB Gremlin API.

## Cosmos DB Gremlin API Analytical Store schema and datatypes

Cosmos DB Gremlin API internally representing Cosmos DB documents based on GraphSON v2 schema using [Gremlin Wire format](https://docs.microsoft.com/en-us/azure/cosmos-db/graph/gremlin-support#gremlin-wire-format).

Reference:[Cosmos Gremlin API back-end JSON](https://github.com/LuisBosquez/azure-cosmos-db-graph-working-guides/blob/master/graph-backend-json.md)  

## Azure Synapse support for Cosmos Gremlin API

There are two ways to access data from Azure Cosmos DB Gremlin API Analytical Store via Synapse Link:
* Using SQL Serverless - use OPENROWSET to query Cosmos Gremlin API container and transorm nested JSON/array data to flatten Gremlin JSON document structure.
* Using Spark - use Spark Graph libraries (such as graphframes, networkx, etc) to transform dataframe data into spesific Graph objects for vertexes and edges and use Cosmos DB SPARK connector to read/write formatted dataframes based on Cosmos Gremlin API JSON document structure for vertex/edge document types.
 

## Example of writing Cosmos DB Gremlin API data using Synapse Spark pool
Describe aproach and samples.

## Example of reading Cosmos DB Gremlin API data using Synapse Spark pool
Describe aproach and samples.

## Example of using Spark Graph libraries to do analytics on Cosmos DB Gremlin API data using Synapse Spark pool
Describe aproach and samples.

## Example of reading Cosmos DB Gremlin API data using Synapse SQL Serverless
Describe aproach and samples.

## Next steps

* [Learn more on Cosmos Gremlin API wire protocol support](/gremlin-support.md)
* [Learn how to query the Cosmos DB Analytical Store with SQL Serverless](/query-cosmos-db-analytical-store.md)
* [Learn how to query the Cosmos DB Analytical Store with Spark 3](how-to-query-analytical-store-spark-3.md)
* [Learn how to query the Cosmos DB Analytical Store with Spark 2](how-to-query-analytical-store-spark.md)
