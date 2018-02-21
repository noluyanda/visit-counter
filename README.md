docker run -dti -p 80:80 --name php -v "$PWD":/var/www/html php:7.0-apache
docker build -t anyname/php:interns-1.0.0 .
Dockerfil
FROM php:7.0-apache
RUN apt update
RUN apt install -y vim
COPY scripts/info.php /var/www/html/
COPY scripts/countlog.txt /var/www/html/
COPY scripts/counter.php /var/www/html/
for more information visit the link 
git@github.com:noluyanda/visit-counter.git
