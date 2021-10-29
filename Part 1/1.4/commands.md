$ docker run -d -it –rm –name test1.4 ubuntu sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
$ docker exec -it bash -c ‘apt-get upgrade && apt-get install curl’
$ docker attach test1.4
