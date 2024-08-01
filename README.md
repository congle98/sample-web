# Simple web app container

Exposes web server on port `8080` as per `./app.js`
See `Dockerfile` for more details

#The Dockerfile is a plain-text document that tells Docker
#how to build the app and dependencies into a Docker image.
```
cat Dockerfile
```
#Build the image
```
docker build -t test:v1 .
```

#List image
```
docker images
```

#Run a container from the image and test the app.
```
docker run -d --name web1 --publish 8080:8080 test:v1
```

#Access http://192.168.64.4:8080

# Exercise
Update content, build and run a new version of sample-web
