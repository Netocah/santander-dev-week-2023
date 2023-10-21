# Santander Dev Week 2023
RESTful Application para a Santander Dev Week
```mermaid
classDiagram
  class User {
    - name: String
    - account: Account
    - features: Feature[]
    - card: Card
    - news: News[]
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

  User "1"*--"1" Account
  User "1"*--"N" Feature
  User "1"*--"1" Card
  User "1"*--"N" News
```
