# Spring Boot v3 Keycloak Integration

Demo project for integrating Keycloak with Spring Boot 3

### Run Keycloak With Docker Image
```shell
docker run -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:21.0.2 start-dev
```

### Endpoints
Anonymous:
```
[GET] http://localhost:8081/api/test/anonymous
```
Admin:
```
[GET] http://localhost:8081/api/test/admin
Authorization - Bearer Token with admin privileges
```
User:
```
[GET] http://localhost:8081/api/test/user
Authorization - Bearer Token with admin or user privileges
```

<hr>
<br>
Medium Article Link: https://medium.com/geekculture/using-keycloak-with-spring-boot-3-0-376fa9f60e0b
