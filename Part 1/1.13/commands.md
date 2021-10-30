$ docker build . -t example-backend && docker run -dit --rm -p 8080 example-backend
$ curl localhost:49156/ping
pong
