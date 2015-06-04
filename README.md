Docker Presentation
===================

A Docker container that sets up my presentation environment.

```
#Build the docker presentation
sudo docker build -t="jamtur01/docker-presentation" .
#Run the container
sudo docker run -p 8000:8000 -p 35729:35729 \
 --name docker_presentation \
-v /Users/james/src/intro-to-docker/images:/opt/presentation/images \
-v /Users/james/src/intro-to-docker/slides:/opt/presentation/slides \
-d jamtur01/docker-presentation
```
