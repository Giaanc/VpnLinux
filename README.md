# VpnLinux
install vpn on linux easy with wget setupvpn.sh type vpn ip/sec with presharedkey

!!!
on windows 8, 8.1, 10 
you need to add this regedit key dword

'IPsec Nat-t' error 
'Windows PowerShell code' after 'restart'
Set-ItemProperty HKLM:\SYSTEM\CurrentControlSet\Services\PolicyAgent -Name AssumeUDPEncapsulationContextOnSendRule -Value 2 -Type DWord
