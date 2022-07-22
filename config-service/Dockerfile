FROM openjdk:17-ea-11-jdk-slim
VOLUME /tmp
ARG JAR_FILE=build/libs/*.jar
COPY ${JAR_FILE} ConfigServer.jar
COPY apiEncryptionKey.jks apiEncryptionKey.jks
ENTRYPOINT ["java","-jar","ConfigServer.jar"]