FROM wordpress:latest
LABEL maintainer="Carlos Ruiz <karlosarr@gmail.com>"
WORKDIR /var/www/html
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
RUN apt-get update -yq \
     && apt-get install curl gnupg -yq \
     && curl -sL https://deb.nodesource.com/setup_8.x | bash \
     && apt-get install nodejs -yq
EXPOSE 80
