# Docker image for Xpra HTML5 Server


## example docker-compose

```
version: '2'

services:
    x:
        image: lanrat/xpra-html5
        networks:
            www_frontend:
        volumes:
            - /etc/localtime:/etc/localtime:ro
            - x_data:/data
        restart: always

networks:
    www_frontend:
        external: true

volumes:
    x_data: {}

```