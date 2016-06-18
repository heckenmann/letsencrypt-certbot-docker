# letsencrypt-docker
Dockerfile to build letsencrypt-image

More information:
https://github.com/certbot/certbot

## Build image
```
docker build --rm -t heckenmann/letsencrypt github.com/heckenmann/letsencrypt-docker
```

## Run container
(You have to set your domain)
```
docker run --it --name letsencrypt -e DOMAIN=<<YOUR_DOMAIN>> heckenmann/letsencrypt
```

## Get files
```
docker cp letsencrypt:/etc/letsencrypt/archive <<your-favorite-directory>>
```
