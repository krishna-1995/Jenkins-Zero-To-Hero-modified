# You can change this base image to anything else
# But make sure to use the correct version of Java
From adoptopenjdk/openjdk11

# Simply add the artifact path to variable
ARG artifacts=target/spring-boot-web.jar

Workdir /opt/app

COPY ${artifacts} app.jar

# This should not be changed
ENTRYPOINT ["java", "-jar", "app.jar"]

