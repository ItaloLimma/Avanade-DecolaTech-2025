# Avanade Decola Tech 2025
Java RESTful API criada para o Avanade Decola Tech

##Diagrama de Classes

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
        - Float balance
        - Float limit
    }
    
    class Feature {
        - String icons
        - String description
    }
    
    class Card {
        - String number
        - Float limit
    }
    
    class News {
        - String icons
        - String description
    }
    
    User "1" *-- "1" Account
    User "1" *-- "n" Feature
    User "1" *-- "1" Card
    User "1" *-- "n" News
```
