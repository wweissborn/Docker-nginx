![CI](https://github.com/wweissborn/nginx/workflows/CI/badge.svg)

# Usage

You need to populate the container with custom NginX configuration files since they have been removed from the image:
```
/etc/nginx/nginx.conf
/etc/nginx/conf.d/*.conf
```
See in this example how to configure the deployment for that purpose:
* https://github.com/secobau/nginx/blob/master/etc/docker/swarm/docker-compose.yaml

You can choose the release and digest to build:
```
ARG digest
ARG tag
FROM nginx:${tag}${digest}
```
