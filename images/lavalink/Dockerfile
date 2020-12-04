FROM adoptopenjdk/openjdk13-openj9:alpine-jre
workdir /opt/Lavalink
COPY Lavalink.jar Lavalink.jar
COPY application.yml .
EXPOSE 2333
CMD ["java", "-jar", "Lavalink.jar"]
