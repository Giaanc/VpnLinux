# on google instance:
southamerica east1 B

# Steps
https://www.youtube.com/watch?v=-y_izsYzPNI

# VpnLinux
Script for automatic setup of an IPsec VPN server on Ubuntu LTS and Debian.
Works on any dedicated server or virtual private server (VPS) except OpenVZ.

# On windows 8, 8.1, 10 
you need to add this regedit key dword

'IPsec Nat-t' error 
'Windows PowerShell code' after 'restart'
Set-ItemProperty HKLM:\SYSTEM\CurrentControlSet\Services\PolicyAgent -Name AssumeUDPEncapsulationContextOnSendRule -Value 2 -Type DWord

# Firewall Rules
https://imgur.com/a/zTQ90DZ

# Steps on CentOS:

on konsole execute

1: 'wget https://raw.githubusercontent.com/Giaanc/VpnLinux/master/vpnsetup.sh'  

2: 'nano -w vpnsetup.sh'

3: remplace with your values

Replace with your own values:
YOUR_IPSEC_PSK - Pre shared key
YOUR_USERNAME - Username
YOUR_PASSWORD - Password

4: 'Ctrl + o'  'enter'  'Ctrl + x'

5: 'sudo sh vpnsetup.sh'

wait 10 minutes

6. on windows 10 , go to network settings -> VPN -> ADD VPN Connection

- vpn provider -> Windows (integrated)
- Connection Name, Server name  <- Own values.
- VPN Type 'L2TP/IPsec Preshared key'
- Username and pass <- Own Values.

Done! , Enjoy

(if you have a error, or does not connect)

'IPsec Nat-t' error
'Windows PowerShell code' after 'restart'
Set-ItemProperty HKLM:\SYSTEM\CurrentControlSet\Services\PolicyAgent -Name AssumeUDPEncapsulationContextOnSendRule -Value 2 -Type DWord

OR 

Go to regedit 

Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\PolicyAgent
add a dword type with a name
'AssumeUDPEncapsulationContextOnSendRule'
set value '2'
Restart

Enjoy!


By Giaanc
