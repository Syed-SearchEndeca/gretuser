FROM openjdk:8-jdk-alpine
RUN addgroup -S spring && adduser -S spring -G spring
USER spring:spring
ENTRYPOINT ["java","-jar","${workspace}\\GreetUser\\target\\GreetUser-0.0.1-SNAPSHOT.jar"]