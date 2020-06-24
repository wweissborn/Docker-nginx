![GitHub release (latest by date)](https://img.shields.io/github/v/release/secobau/nginx?color=Green)

# Usage

You need to populate the container with custom NginX configuration files since they have been removed from the image:
```
/etc/nginx/conf.d/*.conf
```
You can choose the release and digest to build:
```
ARG digest
ARG tag
FROM nginx:${tag}${digest}
```
