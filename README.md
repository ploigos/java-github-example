# Ploigos Example - Java App
A reference application for building and deploying a Java application
using [Ploigos](https://github.com/ploigos).

## Building Locally

To build, run and test this application locally:

```
mvn clean package
buildah bud -t java-app .
podman run --rm -p 8080:8080 java-app
curl http://localhost:8080/fruits/
```

## Source
This is a fork of [rest-json-quickstart](https://github.com/quarkusio/quarkus-quickstarts/tree/master/rest-json-quickstart)
that has been modified to use the [Ploigos Step Runner](https://github.com/ploigos-step-runner).

