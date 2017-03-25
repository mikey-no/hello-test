# hello-world-test
Test Hello World App
Simple as can be.

##References

Dockerizing a Node.js web app:
[https://nodejs.org/en/docs/guides/nodejs-docker-webapp/] (https://nodejs.org/en/docs/guides/nodejs-docker-webapp/)


##Build and image

```
docker build -t node-web-app .
```

##Run the image

```
docker run -p 8000:8080 -d node-web-app
```

run - run
-p port number mapping
    8000 is the external port for the world to use
    8080 is the internal port on the node express app
-d is the display name??