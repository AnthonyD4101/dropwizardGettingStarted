FROM openjdk:11
COPY build/libs/getting-started-1.0-SNAPSHOT-all.jar app.jar
COPY hello-world.yml /hello-world.yml
ENTRYPOINT ["java","-jar","app.jar", "server", "/hello-world.yml"]