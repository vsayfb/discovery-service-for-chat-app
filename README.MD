# Discovery Service For Chat Application

This microservice is part of the _[real-time chat application](https://github.com/vsayfb/real-time-chat-application)._

## Description

This microservice acts as a service registry using Eureka and monitors the status of downstream services registered with it.

## Running the application

#### Development

`docker compose up -d && docker compose logs -f`

#### Testing

`BUILD_TARGET=test docker compose up -d && docker compose logs -f`

#### Production

`docker build -t discovery-ms . && kubectl apply -f deployment.yml`
