setup spring cloud guideline: https://www.baeldung.com/spring-cloud-bootstrapping

start config server first, then discovery server

1.config server will fail when "spring.cloud.config.server.git.uri" not correct
2.http://localhost:8080/book-service/books
  Notice that we are not accessing book service directly on port 8083 but we are going through the gateway(8080) server.
3.http://localhost:8080/rating-service/ratings/all
  Notice that we are not accessing the rating service directly on port 8084 but we are going through the gateway server.