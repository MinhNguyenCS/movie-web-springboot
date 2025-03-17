FROM openjdk:17-alpine
WORKDIR /app
COPY target/movie.jar movie.jar
EXPOSE 8085
ENTRYPOINT [ "java", "-jar", "movie.jar" ]
