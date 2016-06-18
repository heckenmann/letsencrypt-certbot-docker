# letsencrypt-docker
Dockerfile to build letsencrypt-image

## Build image
```
docker build --rm -t heckenmann/letsencrypt github.com/heckenmann/letsencrypt-docker
```

## Run container
(You have to set your domain)
```
docker run --it -e DOMAIN=<<YOUR_DOMAIN>> heckenmann/letsencrypt
```
