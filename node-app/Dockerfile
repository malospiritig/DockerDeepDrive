# Test web-app to use with Pluralsight courses and Docker Deep Dive book
# Linux x64
FROM alpine:3.16

LABEL maintainer="giacio69"

# Install Node and NPM
RUN apk add --update nodejs npm curl

# Copy app to /src
COPY . /src

WORKDIR /src

# Install dependencies
RUN  npm install

EXPOSE 8080

ENTRYPOINT ["node", "./app.js"]
