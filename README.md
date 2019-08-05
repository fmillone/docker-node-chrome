# Dockerfile for Angular 8 tests

Based/forked from  [docker-node-jdk-chrome-firefox](https://bitbucket.org/atlassian/docker-node-jdk-chrome-firefox)

This Dockerfile contains:

* SCM tools
* Node 12.x
* npm latest
* Google Chrome latest
* Bzip2 (for PhantomJS install)
* Zip

## How to build the image
```
docker build -t docker-node-chrome .
```

then use `docker images` to find the image ID.

With `docker run -it <IMAGE_ID>` you can test if your changes are the desired ones.

Then tag it: `docker tag <IMAGE_ID> <YOUR-USER>/docker-node-chrome:latest`

and finally publish it: `docker push <YOUR-USER>/docker-node-chrome`
