
# Docker Commands

## Building the Docker Image

```
docker build -t="governance/base:wildfly8" --rm .
```

## Running the Docker Image
```
docker run -it -p 8080:8080 governance/base:wildfly8
```

Note: the "-p 8080:8080" maps port 8080 in the docker container to port 8080 on your local
host, allowing you to actually point your browser to WildFly 8 at the following URL:

http://localhost:8080

