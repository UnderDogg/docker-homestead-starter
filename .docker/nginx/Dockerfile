FROM nginx:1.15-alpine

RUN apk update && \
    apk upgrade && \
    apk add vim

RUN addgroup -g 1000 -S www-data \
 && adduser -u 1000 -D -S -G www-data www-data

COPY conf/nginx.conf /etc/nginx/nginx.conf
ADD sites-enabled/ /etc/nginx/sites-enabled/

CMD ["nginx", "-g", "daemon off;"]
