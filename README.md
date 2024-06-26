# Projeto Final DIO Bootcamp Santander 2024
Java RESTful API criada para o projeto final DIO.

## Diagrama de Classe

```mermaid

classDiagram
    class User {
        - String name
        - Account account
        - Feature[] features
        - Card card
        - News[] news
    }

    class Account {
        - String number
        - String agency
        - BigDecimal balance
        - BigDecimal limit
    }

    class Feature {
        - String icon
        - String description
    }

    class Card {
        - String number
        - BigDecimal limit
    }

    class News {
        - String icon
        - String description
    }

    User "1" *-- "1" Account
    User "1" *-- "N" Feature
    User "1" *-- "1" Card
    User "1" *-- "N" News
```
