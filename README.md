# hello-world-test
Test Hello World App
Simple as can be.

Wanted to test:
1. creating a simple node js server web application
2. creating a docker image from this
3. running the docker image in a container
4. test the applcation -> open this url http://localhost:8000
5. stoping the container - first by finding the contaner id then stop it based on this id

## References

Dockerizing a Node.js web app:
https://nodejs.org/en/docs/guides/nodejs-docker-webapp/


## Build and image

```
docker build -t node-web-app .
```
all the local files in the directory: .

`-t` tag the image with default tag (i.e. latest) 

## Run the image... creating a container

```
docker run -p 8000:8080 -d node-web-app
```

`run` - run the image as a container

`-p` port number mapping

    `8000` is the external port for the world to use

    `8080` is the internal port on the node express app

`-d` is the display name

## Get the containers ID

```
docker ps
```

## Stop the container

```
docker stop <CONTAINER ID>
```