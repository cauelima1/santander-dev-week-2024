# Santander Dev Week 2024

Java RESTful criada para a Santander Dev Week.

## Diagrama de Classes

``` classDiagram
    class User {
        +String name
        +Account account
        +List<Feature> features
        +Card card
        +List<News> news
    }

    class Account {
        +String number
        +String agency
        +double balance
        +double limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +double limit
    }

    class News {
        +String icon
        +String description
    }

    User "1" --> "1" Account : has
    User "1" --> "N" Feature : includes
    User "1" --> "1" Card : has
    User "1" --> "N" News : includes
```
