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

### Client A
````
cd client-a
cf push
````

### Client B
````
cd client-b
cf push
````

### Client A
````
cd client-c
cf push
````

## Spring Boot Admin
To view the Spring Boot Admin page, load [https://spring-admin-server.cfapps.io) in a browser. You should see client-a, client-b and client-c in the admin console page.

## CF Router
In PCF routes are unique within an organization. Therefore if you get an error on cf push of any service please update <service>/manifest.yml by supplying a unique name for the host attribute. You will also need to update the application.yml file for each client-Z service.
