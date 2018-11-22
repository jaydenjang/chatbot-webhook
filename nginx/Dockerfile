FROM nginx:stable
COPY nginx.conf /etc/nginx/nginx.conf

RUN apt-get update
RUN apt-get -y install vim
RUN apt-get -y install letsencrypt
#RUN letsencrypt certonly --webroot --webroot-path=/usr/share/nginx/html -d geakorea.mooo.com
RUN openssl dhparam -out /etc/ssl/certs/dhparam.pem 2048

EXPOSE 80 443 1337
