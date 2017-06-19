
## Docker Compose Guide
This guide will show you how to make a quick and easy docker compose file to get your container running using the compose tool.


### Creating a compose file
Create a docker-compose.yml file with the following contents:

```
version: '2'

services:
  nginx-php-fpm:
    image: richarvey/nginx-php-fpm:latest
    restart: always
```
You can of course expand on this and add volumes, or extra environment parameters as defined in the [config flags](../config_flags.md) documentation.

### Running
To start the container simply run: ```docker-compose up -d```

### Clean Up
To shut down the compose network and container runt he following command: ```docker-compose down```
