FROM nginx:alpine

COPY default.conf /etc/nginx/conf.d/

COPY index.sh /usr/share/nginx/html/

COPY supervisord.conf /etc/supervisor/supervisord.conf
RUN apk add --no-cache supervisor fcgiwrap shadow && \
    usermod --shell /bin/sh nginx && \
    chmod +x /usr/share/nginx/html/index.sh

CMD ["/usr/bin/supervisord", "-c", "/etc/supervisor/supervisord.conf", "-n"]