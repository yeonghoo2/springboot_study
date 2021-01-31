FROM amazoncorretto:11
WORKDIR /app
COPY build/libs/*.jar app.jar
USER daemon
CMD [ "java", "-jar", "app.jar" ]
