# Getting Started

### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)

### Guides
The following guides illustrate how to use some features concretely:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)
* [Securing a Web Application](https://spring.io/guides/gs/securing-web/)
* [Spring Boot and OAuth2](https://spring.io/guides/tutorials/spring-boot-oauth2/)
* [Authenticating a User with LDAP](https://spring.io/guides/gs/authenticating-ldap/)

curl -X POST "http://localhost:8080/oauth/token" --user clientadmin:123 -d "grant_type=client_credentials&scope=admin"

e.g Output:
{"access_token":"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJzY29wZSI6WyJhZG1pbiJdLCJleHAiOjE1NTUzMzU3OTksImp0aSI6ImYwMDA1ZmFhLTZiZDAtNGJmZC1hNWIzLTI5MjQzNDRlNTk0MCIsImNsaWVudF9pZCI6ImNsaWVudGFkbWluIn0.TvZgM4ezMAPj_2tBuuV3PJ-WjKuF6hpRJ78UxK5LxMardRzuWiyvjDpuWPyyf5GVncN_OX1hfnWdlC7QMtsTjUBbM1Ya73J4_NlpXyrNKDaqbJWYcrlh1z7TFNHIt6ADHHUdTrd5-KEatkbHZ1JiA-hHeiRV00N2k8u5xFLgshM","token_type":"bearer","expires_in":43199,"scope":"admin","jti":"f0005faa-6bd0-4bfd-a5b3-2924344e5940"}

curl "http://localhost:8080/api/users" -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJzY29wZSI6WyJhZG1pbiJdLCJleHAiOjE1NTUzMzU3OTksImp0aSI6ImYwMDA1ZmFhLTZiZDAtNGJmZC1hNWIzLTI5MjQzNDRlNTk0MCIsImNsaWVudF9pZCI6ImNsaWVudGFkbWluIn0.TvZgM4ezMAPj_2tBuuV3PJ-WjKuF6hpRJ78UxK5LxMardRzuWiyvjDpuWPyyf5GVncN_OX1hfnWdlC7QMtsTjUBbM1Ya73J4_NlpXyrNKDaqbJWYcrlh1z7TFNHIt6ADHHUdTrd5-KEatkbHZ1JiA-hHeiRV00N2k8u5xFLgshM"

e.g Output:

[{"name":"adolfo","email":"adolfo@mailinator.com"},{"name":"demigreite","email":"demigreite@mailinator.com"},{"name":"jujuba","email":"jujuba@mailinator.com"}]

