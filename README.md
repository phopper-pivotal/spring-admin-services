# spring-admin-services
A simple set of services that exposes the use of Spring Boot Admin server

## Services (4)
Four services have been provided;
. admin-server
. client-a
. client-b
. client-c

Each service exposes the "/" context with a hello world messsage. Each service has its own unique message.

## Push to Pivotal Cloud Foundry
### Admin Server
````
cd admin-server
cf push
````
