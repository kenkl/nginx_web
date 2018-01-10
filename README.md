# nginx_web
Docker-compose for linuxserver/nginx


This is a simple docker-compose.yml wrapper for the [linuxserver.io nginx Docker image](https://hub.docker.com/r/linuxserver/nginx/). Note that the Dockerfile *doesn't* use the :latest tag.

Note: although the Dockerfile copies info.php into the contaner, the Volume mapping to /docker/nginx overlays it. The COPY in the Dockerfile only serves (for now) to force a creation of a layer, letting the base image have a unique ID.


