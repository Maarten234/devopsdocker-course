```
$ docker run -d -it --rm --name test1.3 devopsdockeruh/simple-web-service:ubuntu
$ docker exec -it test1.3 tail -f ./text.log
$ docker kill test1.3
```
