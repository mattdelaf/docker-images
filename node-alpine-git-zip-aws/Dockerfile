FROM node:12-alpine

LABEL maintainer="Matthieu De La Fourniere<matthieudelafourniere@gmail.com>"
LABEL description="Available on DockerHub at mastymattdelaf/node-alpine-git-zip-aws"

# Install git
RUN apk --no-cache add git

RUN git --version
# Install zip
RUN apk --no-cache add zip

# Install aws-cli
RUN apk -Uuv add groff less python py-pip
RUN pip install awscli
RUN apk --purge -v del py-pip
RUN rm /var/cache/apk/*
