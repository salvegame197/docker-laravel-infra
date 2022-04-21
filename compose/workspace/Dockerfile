FROM php:7.4-fpm-alpine

COPY ./compose/workspace/run.sh /tmp
RUN echo "America/Sao_Paulo" > /etc/timezone

WORKDIR /var/www/html

ENTRYPOINT ["/tmp/run.sh"]
