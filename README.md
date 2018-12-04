
Java Spring Boot rest /get

Dependencies:
  - openjdk 1.8.0
  - apach-maven 3.3.9

```bash
$ java -version
openjdk version "1.8.0_181"
OpenJDK Runtime Environment (build 1.8.0_181-8u181-b13-2~deb9u1-b13)
OpenJDK 64-Bit Server VM (build 25.181-b13, mixed mode)

$ mvn -version
Apache Maven 3.3.9
Maven home: /usr/share/maven
Java version: 1.8.0_181, vendor: Oracle Corporation
Java home: /usr/lib/jvm/java-8-openjdk-amd64/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "linux", version: "4.9.0-8-amd64", arch: "amd64", family: "unix"
```

Build:
```bash
$ mvn clean package
```

Run:
```bash
$ java -jar target/gs-rest-service-0.1.0.jar
```

Test:
```bash
$ curl http://localhost:8080/greeter?name=123
{"id":1,"content":"Hello, 123!"}
```
