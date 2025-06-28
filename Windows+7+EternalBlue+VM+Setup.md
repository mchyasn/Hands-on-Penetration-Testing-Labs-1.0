Free Windows 7 VM:

https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/

Command used:

Set-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Services\LanmanServer\Parameters" SMB1 -Type DWORD -Value 1 -Force