# Microservice Patterns

## Queries in microservices

- Implementing queries in monolithic application is straightforward as it has a single database
- Queries in microservice may retrive data from 
    * Single service
        getConsumerProfile() -> get data from consumer service database
    * Multiple services
        getOrder() -> get data from Order service, Consumer service, etc

### Patterns
    1. API Composition
        - get data by making call to service responsible for the data
        - combine data fetched from different services
    2. Command query responsibility segregation (CQRS)
        - Maintain a view database to support the queries


