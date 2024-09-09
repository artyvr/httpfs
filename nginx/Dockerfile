FROM nginx:alpine
EXPOSE 8080
RUN rm /etc/nginx/conf.d/default.conf
RUN mkdir -p /var/www/static
RUN chmod o+x /var/www/static -R
COPY default.conf /etc/nginx/conf.d