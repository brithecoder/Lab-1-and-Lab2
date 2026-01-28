# Lab 2 API Flexibility Analysis

## The Over-fetching Problem: In your own words, explain the concepts of “over-fetching” and “under-fetching” in the context of a REST API. How does GraphQL’s query language inherently solve this problem?

over fetching is when the endpoint you are hitting returns more data than is needed so you would maybe want to add params to that end point or only add cetain feilds some endpoints wont allow you to return all. Under fetching is when the end point doesnt provide enough data. GraphQL solves this by allowing the client to define a specific query. You ask exactly for the fields you want—nothing more, nothing less. This eliminates over-fetching and allows you to nest related data in a single request, eliminating under-fetching.

## Endpoint and Schema Philosophy: Compare the endpoint structure of a typical REST API with that of a GraphQL API. How does GraphQL’s strongly-typed schema benefit frontend developers?
REST have mutliple endpoints while GraphQL had one .GraphQL uses a Schema Definition Language (SDL) to define exactly what data is available and what type it is (String, Int, Boolean).

## Caching and Complexity: Caching is often cited as a major advantage of REST. Explain why caching is simpler in REST compared to GraphQL. What is a use case where the flexibility of GraphQL might outweigh its caching complexity?

Catching is easier for REST becuase you have mutliple end points so you can search for what you need easier but with GraphQL API you are only hitting one end point for the entire application and it could because very complexed searching for the return or payload of the specific hit of the endpoint you are searching for in the moment. 