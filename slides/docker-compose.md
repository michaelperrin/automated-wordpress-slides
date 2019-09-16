### Setting up Docker containers

Create a `docker-compose.yml` file at the root of the project.

```yaml
services:
  wordpress:
    image: wordpress:5.2-php7.3-fpm-alpine
    # ...

  database:
    image: mysql:5.7
    # ...

  webserver:
    image: nginx:1.14-alpine
    # ...
```
