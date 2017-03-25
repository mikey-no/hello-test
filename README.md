# hello-world-test
Test Hello World App
Simple as can be.

Wanted to test:
<li>creating a simple node js server web application</li>
<li>creating a docker image from this</li>
<li>creating a running the docker image in a container</li>
<li>test the applcation -> open this url http://localhost:8000</li>
<li>stoping the container - first finding the contaner id then stop it</li>

## References

Dockerizing a Node.js web app:
[https://nodejs.org/en/docs/guides/nodejs-docker-webapp/] (https://nodejs.org/en/docs/guides/nodejs-docker-webapp/)


## Build and image

```
docker build -t node-web-app .
```

## Run the image... creating a container

```
docker run -p 8000:8080 -d node-web-app
```

run - run
-p port number mapping
    8000 is the external port for the world to use
    8080 is the internal port on the node express app
-d is the display name??

## Get the containers ID

```
docker ps
```

## Stop the container

```
docker stop <CONTAINER ID>
```