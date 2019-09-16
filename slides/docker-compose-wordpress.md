```yml
wordpress:
  image: wordpress:5.2-php7.3-fpm-alpine
  links:
    - database:mysql
  volumes:
    - wordpress_data:/var/www/html
    - ./wp-content:/var/www/html/wp-content
  restart: always
```
