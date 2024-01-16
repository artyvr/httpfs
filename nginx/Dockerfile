FROM nginx:1.25-alpine
RUN rm /etc/nginx/conf.d/default.conf
RUN mkdir -p /var/www/static
RUN chmod o+x /var/www/static -R
COPY default.conf /etc/nginx/conf.d