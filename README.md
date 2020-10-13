Quarkus study on GraalVM native image using docker

1. mvn package -Pnative -Dquarkus.native.container-build=true

2. docker build -f src/main/docker/Dockerfile.native -t quarkus/hello-quarkus .

3. docker run -i --rm -p 8081:8081 quarkus/hello-quarkus