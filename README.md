# Openvpn-2FA
OpenVPN community server with Google Authenticator</br>
fixed known bugs 


------------------------------------------------------------------------------------------------------------------------
 Added any files
 
 #software.sh
  check os
  and install soft:
    a )epel-release
    b) fail2ban
      1) config fail2ban
      2) start fail2ban (3 or 5 mistake go to jail XD saves from brute force sshd and vsftpd) 
    c) nano 
    d) lsof 
      1) P.S You can use that command  lsof -i -P -n to show active procces which ports 
      
 #install.sh
  install Openvpn, install google-authenticator and adjusts a little
------------------------------------------------------------------------------------------------------------------------

<h1 id="custom-id">Taken from other user <a href='https://github.com/perfecto25/openvpn_2fa'>perfecto25</a></h1>
see https://perfecto25.medium.com/openvpn-community-2fa-with-google-authenticator-4f2a7cb08128
for full description of this setup

------------------------------------------------------------------------------------------------------------------------

uses a modfied version of installation script from https://github.com/angristan/openvpn-install
specifically tailored for Rocky Linux 8tt
