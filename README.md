# Openvpn-2FA
OpenVPN community server with Google Authenticator</br>
fixed known bugs 


------------------------------------------------------------------------------------------------------------------------
 Added any files</br>
 </br>
 #software.sh</br>
  check os</br>
  and install soft:</br>
    a )epel-release</br>
    b) fail2ban</br>
      1) config fail2ban</br>
      2) start fail2ban (3 or 5 mistake go to jail XD saves from brute force sshd and vsftpd) </br>
    c) nano </br>
    d) lsof </br>
      1) P.S You can use that command  lsof -i -P -n to show active procces which ports </br>
      
 <strong>#install.sh<strong></br>
  install Openvpn, install google-authenticator and adjusts a little</br>
------------------------------------------------------------------------------------------------------------------------
</br>
<h1 id="custom-id">Taken from other user <a href='https://github.com/perfecto25/openvpn_2fa'>perfecto25</a></h1></br>
see https://perfecto25.medium.com/openvpn-community-2fa-with-google-authenticator-4f2a7cb08128</br>
for full description of this setup</br>
</br>
------------------------------------------------------------------------------------------------------------------------
</br>
uses a modfied version of installation script from https://github.com/angristan/openvpn-install</br>
specifically tailored for Rocky Linux 8tt</br>
