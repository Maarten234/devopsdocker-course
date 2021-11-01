```
$ docker build . -t example-backend && docker run -dit --rm -p 8080 example-backend
```
As I do this course on a sytem which already has a service installed that uses port 8080 I let docker select an available port. In this case that was port 49154
