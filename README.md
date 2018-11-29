# VpnLinux
Script for automatic setup of an IPsec VPN server on Ubuntu LTS and Debian.
Works on any dedicated server or virtual private server (VPS) except OpenVZ.

# on windows 8, 8.1, 10 
you need to add this regedit key dword

'IPsec Nat-t' error 
'Windows PowerShell code' after 'restart'
Set-ItemProperty HKLM:\SYSTEM\CurrentControlSet\Services\PolicyAgent -Name AssumeUDPEncapsulationContextOnSendRule -Value 2 -Type DWord

# steps:

on konsole execute

1: 'wget https://github.com/Giaanc/VpnLinux/blob/master/vpnsetup.sh'    

(you need wait 10 minute)

2: 'nano -w vpnsetup.sh'

3: remplace with your values

Replace with your own values:
YOUR_IPSEC_PSK - Pre shared key
YOUR_USERNAME - Username
YOUR_PASSWORD - Password


By Giaanc
