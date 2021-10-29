```
$ docker run -p 8080:8080 web-server
$ curl localhost:8080
```
OR
```
$ docker run -dit -p 8080 --name web-server devopsdockeruh/simple-web-service sh -c 'server'
$ curl localhost:8080
```
