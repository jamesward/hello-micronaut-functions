Hello, Micronaut Functions
--------------------------

[![Run on Google Cloud](https://deploy.cloud.run/button.svg)](https://deploy.cloud.run)

Run Locally:
```
./mvnw compile exec:exec
```
Check it out: http://localhost:8080/hello-world

Build Container Locally:
```
./mvnw jib:build compile jib:build -Dimage=gcr.io/${PROJECT_ID}/hello-micronaut-functions
```

Run Container Locally:
```
docker run -it -p8080:8080 gcr.io/jw-demo/hello-micronaut-functions
```
Check it out: http://localhost:8080/hello-world
