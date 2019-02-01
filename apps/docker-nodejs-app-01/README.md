# docker-nodejs-app01

see [`manifest.yml`](manifest.yml)

NOTE: be sure to use a TAGGED docker image

[Benefits of Specifying Tags](https://docs.cloudfoundry.org/devguide/deploy-apps/push-docker.html#tag)

> If you push your Docker image without specifying a tag, you must run cf restage for the changes to take effect.


```sh
# build
docker build -t pfeilbr/docker-nodejs-app01:latest .

# run locally
docker run -it --rm -p 8080:8080 pfeilbr/docker-nodejs-app01:latest

# push docker image
docker push pfeilbr/docker-nodejs-app01:latest

# deploy
cf push
```