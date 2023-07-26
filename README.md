Clean up the whole system and delete every image container etc:

```
docker system prune -a
```

Build a dockerfile and create an image
(execute the below command either from the directory where dockerfile is present, or replace . with path to dockerfile)

```
docker build -t <tag_name> .
```

Run a container from a docker image

```
docker run -it --init -p <host_port>:<container_port><image_name>
```

Bind mount project with docker container

```
docker run -it --init -p 3002:3000 -v "$(pwd)":/developer/nodejs/node-bind-mount-project app-bind-mount-node:latest

## FOR Windows

docker run -it --init -p 3002:3000 -v C:/developer/shiv/projects/containers_demo/node-bind-mount-demo:/developer/nodejs/node-bind-mount-project app-bind-mount-node:latest
```
