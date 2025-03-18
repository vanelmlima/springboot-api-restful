# Springboot API RESTful

API REST na Nuvem usando Spring Boot 3, Java 17 e Railway
(Desafio de projeto Decola Tech 2025)

## URL do deploy
https://springboot-api-restful-vlml-prd.up.railway.app/swagger-ui.html

## Problemas no meu projeto
A aplicação no railway está com um problema que ainda não consegui identificar, ela fica ativa por um tempo mas ao acessar não dá certo.
No log mostra que fica sendo iniciada várias vezes e depois quebra.
Caused by: org.hibernate.exception.GenericJDBCException: Unable to open JDBC Connection for DDL execution [FATAL: password authentication failed for user "postgres"] [n/a]

Esse foi o meu primeiro contato com Java, springboot e tudo o mais.
Não consegui mudar o domínio da aplicação ou implementar algo além das referências devido ao prazo corrido do bootcamp.

Ainda tenho outros projetos para levar à frente no front end, onde tenho mais familiaridade e espero que fiquem melhores.
Assim que possível, gostaria de voltar nesse projeto para trazer uma melhor qualidade e possivelmente mais ideias.

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
