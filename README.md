# SpringBoot2 & Spring Security5 & OAuth2
This project is the basic Oauth2 authentication server implementation.

# Getting Started

```bash
./gradlew clean bootrun
```

Send HTTP request to get "access_token"
* In order to get Authorization header, set ```Basic Auth: username: crown, password: thisissecret```

```bash
curl --location --request POST 'http://localhost:8080/auth/oauth/token' \
--header 'Authorization: Basic Y3Jvd246dGhpc2lzc2VjcmV0' \
--header 'Content-Type: multipart/form-data; boundary=--------------------------101092311882977839110112' \
--form 'grant_type=password' \
--form 'scope=webclient' \
--form 'username=john.carnell' \
--form 'password=password'
```

### Reference Documentation
For further reference, please consider the following sections:

* [Official Gradle documentation](https://docs.gradle.org)
* [Spring Boot Gradle Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.1.12.RELEASE/gradle-plugin/reference/html/)
* [Spring Web](https://docs.spring.io/spring-boot/docs/2.2.4.RELEASE/reference/htmlsingle/#boot-features-developing-web-applications)

### Additional Links
These additional references should also help you:

* [Spring Security 5.0.0.RC1 Released](https://spring.io/blog/2017/11/01/spring-security-5-0-0-rc1-released#password-storage-format)

