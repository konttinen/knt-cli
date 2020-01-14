# Image that wraps the Angular CLI. Used in e.g. various shell commands for
# streamlining the Angular development work.

FROM ubuntu:latest

WORKDIR /app

RUN apt-get update && apt-get install -y \
  curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN apt-get install -y nodejs
RUN (echo N) | npm install -g @angular/cli

CMD ["ng",  "serve", "--host", "0.0.0.0", "--poll", "1000"]
