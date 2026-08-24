FROM maven:3.9-eclipse-temurin-17 AS builder

WORKDIR /build

COPY pom.xml .
COPY src ./src

RUN mvn clean package -DskipTests

FROM eclipse-temurin:17-jre

WORKDIR /app

COPY --from=builder /build/target/JavagotchiWeb-1.0-SNAPSHOT.jar ./javagotchi.jar

EXPOSE 7070

ENTRYPOINT ["java", "-jar", "javagotchi.jar"]