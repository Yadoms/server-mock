# Run wiremock server using standalone jar

```
java -jar wiremock-jre8-standalone-2.31.0.jar --port 8081 --enable-stub-cors
```

# Run wiremock server using docker

## pull image
```
docker pull wiremock/wiremock
```

## run wiremock server 
```
docker run -it --rm -p 8081:8080 --name wiremock-yadoms -v $PWD:/home/wiremock wiremock/wiremock --enable-stub-cors
```

## To display all mocked requests
```
http://localhost:8081/__admin/
```