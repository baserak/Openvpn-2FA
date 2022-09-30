<strong># Openvpn-2FA</strong></br>
OpenVPN community server with Google Authenticator</br>
fixed known bugs 


<h1 id="custom-id">Taked from other user <a href='https://github.com/perfecto25/openvpn_2fa'>perfecto25</a></h1></br>
see https://perfecto25.medium.com/openvpn-community-2fa-with-google-authenticator-4f2a7cb08128</br>
for full description of this setup</br>
</br>

------------------------------------------------------------------------------------------------------------------------------
<h1>Known bugs</h1></br>
<p> If you have a proxy in your company, plese configure install.sh</br>
 change install.sh on 60 line to like that </br> 
 IP=$(curl -x "http://{proxi_ip_address}:{proxy_port}"-4 "http://icanhazip.com" )</br>
 or</br>
 IP=$(curl -x "http://{user}:{pwd}@{127.0.0.1}:{1234}"-4 "http://icanhazip.com" )</br>
 if you have a proxy with login and pass </br>
 </br>
and config file /etc/wgetrc</br>
in line 78-79</br>
https_proxy = http:/{proxi_ip_address}:{proxy_port}</br>
http_proxy = http://{proxi_ip_address}:{proxy_port}</br>
if you need ftp uncomment line 80</br>
#ftp_proxy = http://{proxi_ip_address}:{proxy_port}</br>


</p>
------------------------------------------------------------------------------------------------------------------------------

</br>
uses a modfied version of installation script from https://github.com/angristan/openvpn-install</br>
specifically tailored for Rocky Linux 8tt</br>


<h1 id="custom-id"><strong>Manual </strong></h1></br>
 First run software.sh </br>
 Next run install.sh </br>
 Open manual from perfecto25 <a href='https://perfecto25.medium.com/openvpn-community-2fa-with-google-authenticator-4f2a7cb08128'>LINK TO MANUAL</a> </br>
 for full description of this setup </br>
 
------------------------------------------------------------------------------------------------------------------------
 Added any files</br>
 </br>
 <h2><strong>#software.sh</strong></h2></br>
  check os</br>
  and install soft:</br>
    a )epel-release</br>
    b) fail2ban</br>
      1) config fail2ban</br>
      2) start fail2ban (3 or 5 mistake go to jail XD saves from brute force sshd and vsftpd) </br>
    c) nano </br>
    d) lsof </br>
      1) P.S You can use that command  lsof -i -P -n to show active procces which ports </br>
      
 <h2><strong>#install.sh</strong></h2></br>
  install Openvpn, install google-authenticator and adjusts a little</br>
  
 <h2><strong>#manage.sh</strong></h2></br>
  have 2 arg</br>
  usage:</br>
   ./manage.sh create/revoke <username></br>
  ./manage.sh status</br>

 

 <h2><strong>#statusovpn.sh</strong></h2></br>
 Show status Openvpn
 
 <h2><strong>#restatusovpn.sh</strong></h2></br>
 Restart Openvpn

 <h2><strong>#startovpn.sh</strong></h2></br>
 Start Openvpn

 <h2><strong>#stopovpn.sh</strong></h2></br>
 Stop Openvpn

 <h2><strong>#editserver.sh</strong></h2></br>
  Open server.conf with nano 
