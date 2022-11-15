# spring-swagger
#enable swagger
spring:
  profiles:
    include:
      - swagger
      
#dependency for swagger
<dependency>
    <groupId>io.springfox</groupId>
    <artifactId>springfox-boot-starter</artifactId>
    <version>3.0.0</version>
</dependency>

#check swagger ui
http://localhost:8080/swagger-ui/

#exception : org.springframework.context.ApplicationContextException: Failed to start bean 'documentationPluginsBootstrapper'; nested exception is java.lang.NullPointerException
  mvc:
    path match:
      matching-strategy: ant_path_matcher
