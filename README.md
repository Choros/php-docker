# Alpine Docker PHP

[![Docker Repository on Quay](https://quay.io/repository/choros/php-docker/status "Docker Repository on Quay")](https://quay.io/repository/choros/php-docker)

PHP Docker image base on Alpine Linux

## Set timezone

Add to yours Dockerfile

```
# Configure timezone
 RUN apk --no-cache add tzdata \
     && cp /usr/share/zoneinfo/Europe/Warsaw /etc/localtime \
     && echo "Europe/Warsaw" > /etc/timezone \
     && apk del tzdata
```


