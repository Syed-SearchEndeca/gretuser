FROM openjdk:8-jdk-alpine
RUN addgroup -S spring && adduser -S spring -G spring
USER spring:spring
ARG JAR_FILE="${workspace}\\GreetUser\\target\\GreetUser-0.0.1-SNAPSHOT.jar"
ENV JAR_FILE ${JAR_FILE}
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]