FROM registry.digitalocean.com/supernice-k8s-registry/nginx:55fee892733901fbdea9b91d38e64e043e5f8d73
ADD backend/index.php /var/www/html/index.php
ADD backend/pools_www.conf /etc/php/7.3/fpm/pool.d/www.conf
EXPOSE 80
CMD ["/usr/bin/supervisord","-n","-c","/etc/supervisord.conf"]
