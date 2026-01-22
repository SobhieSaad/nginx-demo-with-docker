# A node js application serving a static HTML file

## Using nginx to configure the links and forward the requests

### Install nginx on mac
#### brew install nginx
#### Find nginx location:
#### - whereis nginx OR nginx -V
#### Then locate the `nginx.conf` file:
#### - open /opt/homebrew/etc/nginx/nginx.conf 
##
### Start docker containers from the image:
#### docker-compose up --build -d

### Moving to Secruity connection we need SSL certificates with openssl
#### openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout nginx-selfsigned.key -out nginx-selfsigned.crt