# Docker image for Xpra HTML5 Server


## example docker-compose

```
version: '2'

services:
    x:
        image: lanrat/xpra-html5
        volumes:
            - /etc/localtime:/etc/localtime:ro
            - x_data:/data
        restart: always
        ports:
            - 80:80

volumes:
    x_data: {}

```
