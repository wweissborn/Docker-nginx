# Usage

You need to populate the container with a custom NginX configuration since it has been removed from the image:
`/etc/nginx/nginx.conf`

In that custom configuration you need to *include* the following files:
```
    include /etc/nginx/conf.d/configs/*.conf;
    include /etc/nginx/conf.d/secrets/*.conf;
```
