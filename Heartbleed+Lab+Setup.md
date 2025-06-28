iso download link:

http://old-releases.ubuntu.com/releases/12.04.1/

Commands used:

apt-get install apache2.2-common

a2enmod ssl

service apache2 restart

mkdir /etc/apache2/ssl

openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/apache2/ssl/webserver.key -out /etc/apache2/ssl/webserver.crt

ifconfig eth1 up

dhclient eth1

ifconfig

vi /etc/apache2/sites-available/default-ssl

apt-get install apache2-mpm-prefork

a2ensite default-ssl

service apache2 reload





