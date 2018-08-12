FROM dockerliweipei/xdebug:nginx7.1
ADD ./tools/nginx.conf /etc/nginx/nginx.conf
RUN  apt install -y net-tools iputils-ping
EXPOSE 80
CMD /usr/local/sbin/php-fpm  -D&&nginx -g 'daemon off;'
