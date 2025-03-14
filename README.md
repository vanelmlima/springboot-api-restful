# Springboot API RESTful

API REST na Nuvem usando Spring Boot 3, Java 17 e Railway
(Desafio de projeto Decola Tech 2025)

### Diagrama de classe
``` mermaid
classDiagram
class User {
-String name
-Account account
-Feature[] features
-Card card
-News[] news
}

class Account {
-String number
-String agency
-Number balance
-Number limit
}

class Feature {
-String icon
-String description
}

class Card {
-String number
-Number limit
}

class News {
-String icon
-String description
}

User "1" *-- "1" Account
User "1" *-- "N" Feature
User "1" *-- "1" Card
User "1" *-- "N" News

```
