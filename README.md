# JmsApp_embedded
App using a simple API with embedded ActiveMQ. Delivers messages to topic subscribers.

## To run:
  - `mvn clean install`
  - `docker-compose up`
  
Exposed endpoints:

`GET  8080/all`  returns all messages from an in-memory DB 

`POST 8080/send/{topic}/{message}`  sends {message} to {topic}

  **registered topics: A, BC** every other topic will return 404
