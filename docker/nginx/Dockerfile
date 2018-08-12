FROM dockerliweipei/xdebug:nginx7.0
ADD ./tools/nginx.conf /etc/nginx/nginx.conf
RUN  apt install -y net-tools iputils-ping
RUN chmod -R 777 /var/www/html/app/storage
EXPOSE 80
CMD /usr/local/sbin/php-fpm  -D&&nginx -g 'daemon off;'
