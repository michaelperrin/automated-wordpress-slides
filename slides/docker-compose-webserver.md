```yml
webserver:
  image: nginx:1.14-alpine
  links:
    - wordpress
  volumes:
    - wordpress_data:/var/www/html
    - ./docker/nginx/website.conf:/etc/nginx/conf.d/default.conf:ro
    - ./wp-content:/var/www/html/wp-content
  ports:
    - ${WEBSERVER_PORT}:80
```
