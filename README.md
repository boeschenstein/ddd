# DDD - Domain Driven Design

See also: Clean Architecture: <https://github.com/boeschenstein/clean-architecture>

## Compare DDD - Clean Architecture

Topic                     | DDD                | Clean Architecture
--                        | --                 | -- 
Most outer layer          | Web, Api, Gui, ... | Web, Api, Gui, ...
Application Service Layer | required           | relaxed (add more layers if you need it)
Domain Service Layer      | required           | recommended
Infrastructure Layer 1)   | x                  | x
Most inner layer          | Entity             | Entity
Domain Events             | required           | recommended
CQS                       | required           | recommended
Seedwork                  | required           | recommended

`1) Dependency inversion: Infrastructure Layer implements the (example: Repository) Interface, defined in Domain Service Layer`

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
