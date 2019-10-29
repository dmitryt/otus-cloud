FROM alpine:3.10.3
RUN apk update && \
    apk add nginx && \
    mkdir -p /run/nginx && \
    mkdir -p /var/www/html

COPY http.conf /etc/nginx/conf.d/http.conf

CMD ["nginx", "-g", "daemon off;"]