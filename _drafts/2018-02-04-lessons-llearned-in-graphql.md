---
layout: post
title: Lalalala
comments: False
---

In a world where combining fields and features from different places is really annoying and difficult work, GraphQL comes along to save the day.

## GraphQL

[GraphQL](http://graphql.org/) is "a query language for your API". What does this mean? When writing an API, the most common complaint from clients is that the API isn't verbose enough to fit their needs. The most common complaint from the maintainers of the API is that it's a hassle to try to accept every type of request a client could ask for. GraphQL fixes this problem.

For example, let's say that I run a fruit market. My fruit market sells all types of fruit, but we try our best to sell our fruit in season. What APIs should we expose?

1. An endpoint to buy fruit. Let's call this `POST /orders`
2. An endpoint to get more info about a fruit, to see fruit ratings and reviews, recipies etc. Let's call this `GET /fruits/{fruit}`
3. An inventory API that keeps track of what we have in stock. Let's call this `GET /fruits`.
4. An endpoint for a user to see their profile and cart. Let's call this `GET /users/{userId}`

Unfortunately, this is just the tip of the iceberg for the endpoints our little produce market may want to expose. A good initial rule of thumb for an API is: 
> A resource does not have to be based on a single physical data item. For example, an order resource might be implemented internally as several tables in a relational database, but presented to the client as a single entity. Avoid creating APIs that simply mirror the internal structure of a database. The purpose of REST is to model entities and the operations that an application can perform on those entities. A client should not be exposed to the internal implementation. [[1]](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

However, Microsoft also notes that: 
> Avoid requiring resource URIs more complex than collection/item/collection. [[1]](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

So let's try and stick to that rule and not make our relationships too deep. Meaning, we should strive to have simple relationships between our collections. For example if we were interested in seeing how many bananas a user bought in the past month we may do something like `/users/5/