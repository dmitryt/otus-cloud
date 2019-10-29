FROM alpine:3.10.3
RUN apk update && \
    apk add nginx && \
    mkdir -p /run/nginx && \
    mkdir -p /usr/local/nginx/html

COPY http.conf /etc/nginx/conf.d/http.conf
COPY index.html /usr/local/nginx/html/index.html

CMD ["nginx", "-g", "daemon off;"]