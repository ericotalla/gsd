# Test web app that returns the name of the host/pod/container servicing req
FROM node:current-alpine

LABEL org.opencontainers.image.title="Hello Docker Learners!" \
      org.opencontainers.image.description="Web server showing host that responded" \
      org.opencontainers.image.authors="@erictalla"

# creating my working directory
WORKDIR /usr/bin/app

#copy curent directory to working directory

COPY . /usr/bin/app

# install dependencies from package.json

RUN npm install

#Command for container to execute

ENTRYPOINT [ "node","app.js" ]
