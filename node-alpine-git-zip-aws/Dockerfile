FROM node:14-alpine

LABEL maintainer="Matthieu De La Fourniere<matthieudelafourniere@gmail.com>"
LABEL description="Available on DockerHub at mastymattdelaf/node-alpine-git-zip-aws"

# Install git
RUN apk --no-cache add git

RUN git --version

# Install zip
RUN apk --no-cache add zip

# Install aws-cli
# Found on https://stackoverflow.com/questions/61918972/how-to-install-aws-cli-on-alpine
RUN apk add --no-cache \
        python3 \
        py3-pip \
    && pip3 install --upgrade pip \
    && pip3 install --no-cache-dir \
        awscli \
    && rm -rf /var/cache/apk/*
