# Santander Dev Week 2025
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        - String name
        - Account account
        - Card card
        - List~Feature~ features
        - List~News~ news
    }

    class Account {
        - String number
        - String agency
        - double balance
        - double limit
    }

    class Feature {
        - String icon
        - String description
    }

    class Card {
        - String cardNumver
        - double limit
    }

    class News {
        - String icon
        - String description
    }

    User *--> Account
    User *--> Card
    User *--> Feature : has
    User *--> News : has
```
