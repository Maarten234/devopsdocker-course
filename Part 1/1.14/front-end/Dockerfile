FROM ubuntu:latest
WORKDIR /usr/src/app
EXPOSE 5000
# As described in the back-end commands.md file. I have already a service running at port 8080. The back-end container port 8080 was accessible via port 49154 during the excercis
ENV REACT_APP_BACKEND_URL=http://localhost:49154
COPY ./example-frontend/ .
RUN apt-get update && apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_14.x | bash 
RUN apt install -y nodejs
RUN npm install
RUN npm run build
RUN npm install -g serve
CMD ["serve","-s","-l","5000","build"]
