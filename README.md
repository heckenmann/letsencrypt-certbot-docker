# letsencrypt-docker
Dockerfile to build letsencrypt-image

## Build image
```
docker build --rm -t heckenmann/letsencrypt github.com/heckenmann/letsencrypt-docker
```

## Run container
(You have to set your domain and the path where the certs have to be)
```
docker run --it --name letsencrypt -v <<path-where-the-certs-should-be-later>>:/etc/letsencrypt/archive -e DOMAIN=<<YOUR_DOMAIN>> heckenmann/letsencrypt
```
