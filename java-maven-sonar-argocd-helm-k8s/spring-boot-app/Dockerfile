# You can change this base image to anything else
# But make sure to use the correct version of Java
From adoptopenjdk/openjdk11:aarch64-ubuntu-jre-11.0.30_5-ea-beta-nightly

# Simply add the artifact path to variable
ARG artifacts=target/spring-boot-web.jar

Workdir /opt/app

COPY ${artifacts} app.jar

# This should not be changed
ENTRYPOINT ["java", "-jar", "app.jar"]

