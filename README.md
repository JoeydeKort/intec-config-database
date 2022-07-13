## Intec-config-database
***
### Introduction
This is the Git repository used by the `config-server` of the 9 microservices applications at 
https://github.com:JoeydeKort/intec-config-database.git.
***
### Project structure
The full application consists of 9 separated applications. These all work together to get the end result.
- `intec-admin-application`
- `intec-business-application`
- `intec-config-database`
- `intec-config-server`
- `intec-discovery-server`
- `intec-monitor-application`
- `intec-news-application`
- `intec-proxy-server`
- `intec-website-application`
***
### Prerequisites
- H2 database
  To make sure everything work properly you need to have the `intec-config-database` connect with `intec-config-server`.
  The `intec-config-server` will connect to the git repository of the `intec-config-database`.
***

### running the applications
There is a sequence for running the applications.
1) Start the `discovery-server` application (Eureka app)
2) Start the `config-server` application (Spring Cloud Config app)
3) Start the`business-application` microservice (REST app)
4) Start the`admin-application` microservice (Vaadin app)
5) Start the `news-application` microservice (Vaadin app)
6) Start the `website-application` microservice (Vaadin app)
7) Start the `proxy-server` application (Zuul app)

Then open de browser on `localhost:8080` to run the full application.
***

