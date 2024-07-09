# MultiArch Image Build demo 

docker buildx create --use
docker buildx ls

### Push to repository ###

```
docker login

docker tag nodejs-multiarch-example username/nodejs-multiarch-example:latest
docker push username/nodejs-multiarch-example:latest

docker buildx build --platform linux/amd64,linux/arm64 -t username/nodejs-multiarch-example --push .

docker buildx imagetools inspect username/nodejs-multiarch-example

```





