# Santander Dev Week 2023
Java Restful API criada para satander dev week.

## Diagrama de Classes

```mermaid
classDiagram
  class User {
    - name: String
    - acount: Account
    - features: List<Feature>
    - card: Card
    - news: List<News>
  }
  
  class Account {
    - number: String
    - agency: String
    - balance: String
    - limit: String
  }
  
  class Feature {
    - icon: String
    - description: String
  }
  
  class Card {
    - number: String
    - limit: String
  }
  
  class News {
    - icon: String
    - description: String
  }
  
  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1" Card
  User "1" *-- "N" News

```
