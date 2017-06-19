![docker hub](https://img.shields.io/docker/pulls/richarvey/nginx-php-fpm.svg?style=flat-square)
![docker hub](https://img.shields.io/docker/stars/richarvey/nginx-php-fpm.svg?style=flat-square)
![Travis](https://img.shields.io/travis/ngineered/nginx-php-fpm.svg?style=flat-square)

## Overview
This is a Dockerfile/image to build a container for nginx and php-fpm.
The container also has the ability to update templated files with variables passed to docker in order to update your code and settings. 
There is support for lets encrypt SSL configurations, custom nginx configs, core nginx/PHP variable overrides for running preferences, X-Forwarded-For headers and UID mapping for local volume support.

If you have improvements or suggestions please open an issue or pull request on the GitHub project page.

### Versioning
| Docker Tag | GitHub Release | Nginx Version | PHP Version | Alpine Version |
|-----|-------|-----|--------|--------|
| latest | Master Branch |1.13.1 | 5.6 | 3.4 |

### Links
- [https://github.com/oniksfly/nginx-php-fpm](https://github.com/oniksfly/nginx-php-fpm)
- [https://registry.hub.docker.com/u/richarvey/nginx-php-fpm/](https://hub.docker.com/r/onxsol/nginx-php-fpm/)

## Quick Start
To pull from docker hub:
```
docker pull onxsol/nginx-php-fpm:latest
```
### Running
To simply run the container:
```
sudo docker run -d onxsol/nginx-php-fpm
```

You can then browse to ```http://<DOCKER_HOST>``` to view the default install files. To find your ```DOCKER_HOST``` use the ```docker inspect``` to get the IP address (normally 172.17.0.2)

For more detailed examples and explanations please refer to the documentation.
## Documentation

- [Building from source](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/building.md)
- [Versioning](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/versioning.md)
- [Config Flags](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/config_flags.md)
- [User / Group Identifiers](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/UID_GID_Mapping.md)
- [Custom Nginx Config files](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/nginx_configs.md)
 - [REAL IP / X-Forwarded-For Headers](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/nginx_configs.md#real-ip--x-forwarded-for-headers)
- [Scripting and Templating](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/scripting_templating.md)
 - [Environment Variables](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/scripting_templating.md#using-environment-variables--templating)
- [Lets Encrypt Support](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/lets_encrypt.md)
 - [Setup](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/lets_encrypt.md#setup)
 - [Renewal](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/lets_encrypt.md#renewal)
- [PHP Modules](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/php_modules.md)
- [Logging and Errors](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/logs.md)

## Guides
- [Running in Kubernetes](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/guides/kubernetes.md)
- [Using Docker Compose](https://github.com/ngineered/nginx-php-fpm/blob/master/docs/guides/docker_compose.md)

## History
- Build on [ngineered's solution](https://github.com/ngineered/nginx-php-fpm)