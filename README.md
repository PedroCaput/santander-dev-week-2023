# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        -String name
        -Account account
        -List<Feature> features
        -Card card
        -List<News> news
    }
    class Account {
        -String number
        -String agency
        -float balance
        -float limit
    }
    class Feature {
        -String icons
        -String description
    }
    class Card {
        -String number
        -float limit
    }
    class News {
        -String icons
        -String description
    }

    User "1" *-- "1" Account
    User "1" *-- "n" Feature
    User "1" *-- "1" Card
    User "1" *-- "n" News

```
