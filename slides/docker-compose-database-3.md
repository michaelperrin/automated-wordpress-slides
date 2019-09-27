<pre><code class="yml" data-line-numbers="6-10" data-trim data-noescape>
database:
  image: mysql:5.7
  restart: always
  volumes:
      - db_data:/var/lib/mysql
  environment:
    MYSQL_ROOT_PASSWORD: ${MYSQL_ROOT_PASSWORD}
    MYSQL_DATABASE: ${MYSQL_DATABASE}
    MYSQL_USER: ${MYSQL_USER}
    MYSQL_PASSWORD: ${MYSQL_USER_PASSWORD}
  ports:
    - 3306:3306
</code></pre>