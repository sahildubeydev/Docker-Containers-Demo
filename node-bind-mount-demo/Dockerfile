FROM node

WORKDIR /developer/nodejs/node-bind-mount-project

COPY . .

RUN npm ci

ENV PORT 3000

CMD ["npm", "start"]

#docker run -it --init -p 3002:3000 -v "$(pwd)":/developer/nodejs/node-bind-mound-project app-bind-mount-node:latest
## FOR WINDOWS see below
#docker run -it --init -p 3002:3000 -v C:/developer/shiv/projects/containers_demo/node-bind-mount-demo:/developer/nodejs/node-bind-mount-project app-bind-mount-node:latest