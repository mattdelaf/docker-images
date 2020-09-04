# To build and push an image to DockerHub

Ex for `node-alpine-git-zip-aws`

```
cd node-alpine-git-zip-aws

docker login # make sure you login to docker account

docker build . -t mastymattdelaf/node-alpine-git-zip-aws

docker push mastymattdelafnode-alpine-git-zip-aws
```
