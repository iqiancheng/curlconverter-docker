# curlconverter-docker
curlconverter host via docker &amp; docker-compose 

<https://hub.docker.com/r/programyun1/curlconverter>
```yml
version: '2'
services:
  curlconverter:
    container_name: curlconverter
    image: programyun1/curlconverter:latest
    restart: unless-stopped
    ports:
      - 80:80
    environment:
      TZ: Asia/Shanghai
    volumes:
      - /etc/localtime:/etc/localtime:ro
```
