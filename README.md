# MultiArch Image Build demo 

### using buildx ###

```
docker buildx create --use
docker buildx ls

docker login

docker tag nodejs-multiarch-example username/nodejs-multiarch-example:latest
docker push username/nodejs-multiarch-example:latest

docker buildx build --platform linux/amd64,linux/arm64 -t username/nodejs-multiarch-example --push .

docker buildx imagetools inspect username/nodejs-multiarch-example

```





