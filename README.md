# base image

1. Run ```$ mkdir log log/nginx log/php7 public``` in your project directory.

2. Create a `docker-compose.yml`:

```
web:
  build: dockercmsimages/base
  ports:
    - 80:80
  volumes:
    - ./log:/var/log
    - ./public:/app/public
```
