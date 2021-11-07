```
$ docker build ./back-end/. -t example-backend && docker run -dit --rm -p 8080 example-backend
$ docker ps
CONTAINER ID   IMAGE             COMMAND                 CREATED         STATUS         PORTS                                         NAMES
2bc2eeb161c7   example-backend   "/bin/sh -c ./server"   4 minutes ago   Up 4 minutes   0.0.0.0:49153->8080/tcp, :::49153->8080/tcp   sweet_moore
```
edit ./front-end/Dockerfile and put in:
ENV REACT_APP_BACKEND_URL=http://localhost:49153
```
$ docker build ./front-end/ -t example-frontend && docker run -it --rm -p 5000:5000 example-frontend
```
