FROM maven:3.8.3-openjdk-17

WORKDIR /app

COPY . .

RUN mvn clean install

COPY /target/observability-0.0.1-SNAPSHOT.jar /app

EXPOSE 8080

CMD ["java", "-jar", "app.jar"]