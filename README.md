# DDD - Domain Driven Design

See also: Clean Architecture: <https://github.com/boeschenstein/clean-architecture>

## Introduction

- STOP dogmatic Domain Driven Design: <https://piped.kavin.rocks/watch?v=8XmXhXH_q90>
- Domain-Driven Design in 150 Seconds: <https://piped.kavin.rocks/watch?v=8Z5IAkWcnIw>

## Domain Model

- https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/microservice-domain-model
- Good DDD example: https://github.com/dotnet-architecture/eShopOnContainers/tree/dev/src/Services/Ordering

### Domain Entity Pattern

- https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/microservice-domain-model#the-domain-entity-pattern
- Entities (Properties only) + Logic = Domain Entities

### Rich Model vs Anemic Model

- https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/microservice-domain-model#rich-domain-model-versus-anemic-domain-model
- Good example (entities contain logic): https://github.com/dotnet-architecture/eShopOnContainers/tree/dev/src/Services/Ordering

## Layers

- https://learn.microsoft.com/en-us/dotnet/architecture/microservices/multi-container-microservice-net-applications/microservice-application-design

### Dependency Inversion: Repository contracts (interfaces) in the domain model layer

- https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/seedwork-domain-model-base-classes-interfaces#repository-contracts-interfaces-in-the-domain-model-layer

## Compare DDD - Clean Architecture

Topic                     | DDD                | Clean Architecture
--                        | --                 | -- 
Most outer layer          | Web, Api, Gui, ... | Web, Api, Gui, ...
Application Service Layer | ?                  | relaxed (add more layers if you need it)
Domain Service Layer      | ?                  | recommended
Infrastructure Layer 1)   | x                  | x
Most inner layer          | Domain Entity      | Domain Entity
Domain Events             | required           | recommended
CQS                       | required           | recommended
Seedwork                  | required           | recommended

`1) Dependency inversion: Infrastructure Layer implements the interface (example: Repository). The interface is defined in Domain Service Layer`

## Information

- Books
    - Martin Fowler: Patterns of Enterprise Application Architecture
    - Eric Evans: Domain-Driven Design
- PluralSight
    - Julie Lerman, Ardalis: https://app.pluralsight.com/library/courses/fundamentals-domain-driven-design/
    - https://app.pluralsight.com/library/courses/domain-driven-design-in-practice
    - Dino Esposito: https://app.pluralsight.com/library/courses/modern-software-architecture-domain-models-cqrs-event-sourcing
    - https://app.pluralsight.com/paths/skill/microservices-architecture
- Web
    - Martin Fowler: https://martinfowler.com
    - Greg Young: CQRS, Eventsourcing
    - Udi Dahan: https://udidahan.com
- Seedwork: https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/seedwork-domain-model-base-classes-interfaces
