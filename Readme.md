# Test application execution

Spring Boot application is actually part of the **main** submodule.
This means you have to configure main SpringBoot class in this submodule.
You can read on how to configure main SpringBoot application class in official documentation 
of SpringBoot Gradle plugin: https://docs.spring.io/spring-boot/docs/current/gradle-plugin/reference/htmlsingle/#packaging-executable.configuring.main-class

1) Build project

- build root project or `./gradlew clean build`
- build main project or `./gradlew :main:build`
- execute task bootJar `./gradlew bootJar` or `./gradlew :main:bootJar`

2) Execute jar 

Note your SpringBoot jar is called as its project -> **main-1.0-SNAPSHOT.jar** and ist located inside of the main subproject build.

`java -jar code/main/build/libs/main-1.0-SNAPSHOT.jar`