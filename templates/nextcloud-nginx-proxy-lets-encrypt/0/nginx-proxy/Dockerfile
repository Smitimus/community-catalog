FROM jwilder/nginx-proxy:alpine

COPY uploadsize.conf /etc/nginx/conf.d/

COPY proxytimeout.conf /etc/nginx/conf.d/

RUN { \
      echo 'server_tokens off;'; \
      echo 'client_max_body_size 100m;'; \
    } > /etc/nginx/conf.d/my_proxy.conf