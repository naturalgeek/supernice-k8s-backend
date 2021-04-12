FROM registry.digitalocean.com/supernice-k8s-registry/nginx:76f510f0e86ffd8a9f5641863d2c6a569caa3416
RUN echo "very simple backend application" > /var/www/html/index.html
ADD backend/index.php /var/www/html/info.php
ADD backend/pools_www.conf /etc/php/7.3/fpm/pool.d/www.conf
EXPOSE 80
CMD ["/usr/bin/supervisord","-n","-c","/etc/supervisord.conf"]
