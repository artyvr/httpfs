FROM nginx:alpine

EXPOSE 8080

RUN rm /etc/nginx/conf.d/default.conf

RUN mkdir -p /var/www/static
RUN chmod o+x /var/www/static -R

RUN mkdir -p /var/www/images
RUN chmod o+x /var/www/images -R

RUN mkdir -p /var/www/icons
RUN chmod o+x /var/www/icons -R

RUN mkdir -p /var/www/videos
RUN chmod o+x /var/www/videos -R

RUN mkdir -p /var/www/audio
RUN chmod o+x /var/www/audio -R

COPY default.conf /etc/nginx/conf.d