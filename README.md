# psjavamicroservspringcloud_nt

## 2. Introduction
### 2 What are microservices
"loosely coupled service oriented architecture with bounded context" 

### 4 What is Spring Cloud
### 5 What is Spring Boot
Adv:
- Offers opinionated runtime for Spring.  
- Convention over configuration
- Opinions can be overriden

### 6 DEMO
```
localhost:8080/beans
localhost:8080/health
localhost:8080/mappings,trace
```
## 3. Simplifying Environment Management with Centralized Configuration
### 3 Problems with the Status Quo
Problems
- Local configuration files fall out of sync
- No history of changes with env variables
- Configuration changes require restart
- Sensitive info

### 4 Create a Config Server
HTTP access to git or file based configurations

steps:
- generate scaffold folding
- See POM dependency on spring-cloud-config-server
- Add @EnableConfigServer annotation.
- create application properties(YAML) with server port
