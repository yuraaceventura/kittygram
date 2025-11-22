FROM nginx:1.22.1

COPY nginx.conf /etc/nginx/nginx.conf

RUN mkdir -p /static /media && \
    chown -R nginx:nginx /static /media && \
    chmod -R 755 /static /media

RUN mkdir -p /var/log/nginx && \
    chown -R nginx:nginx /var/log/nginx

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]