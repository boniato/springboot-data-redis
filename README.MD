# SpringBoot Data Redis Example

This project is an example of SpringBoot Data Redis

# Technologies

* [Java 8](http://java.oracle.com)
* [embedded gradle](https://gradle.org/)
* [spring-boot](http://projects.spring.io/spring-boot/)

# Redis library
**build.gradle**

```groovy
    compile('org.springframework.boot:spring-boot-starter-data-redis')
    compile 'org.springframework.data:spring-data-redis'
    compile group: 'redis.clients', name: 'jedis', version: '2.9.0'
    compile group: 'it.ozimov', name: 'embedded-redis', version: '0.7.1'
```


You can test by using curl, URL, Swagger

# How to Run
**Curl**
```groovy
    curl -X GET --header 'Accept: application/json' 'http://localhost:8081/api/user/userid'
```

**Request URL**
```groovy
    http://localhost:8081/api/user
    http://localhost:8081/api/user/userid
```

**Swagger**
```groovy
    http://localhost:8081/swagger-ui.html
```

# Run test

The repository contains some test cases to cover both api test and repository test.

    ./gradlew test
