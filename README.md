# ssh,ssl,vpn tunnel service + ocs panel

Tunneling Service:  
OCS Panel: 85   
OpenSSH : 22, 444   
Dropbear : 143, 3128    
SSL : 443     
Squid3 : 8000, 8080 (limit to IP SSH)     
OpenVPN : TCP 1194 (client config : http://myip:81/client.ovpn)    
badvpn : badvpn-udpgw port 7300    
nginx : 81

__________________________________________________
# **วิธีติดตั้ง ( Debian 7,8 เท่านั้น )**

- **OCS Panel Only**
```
wget https://raw.githubusercontent.com/ZENON-VPN/ocs-panel/master/OCSAutoScrptz.sh && chmod +x OCSAutoScrptz.sh && ./OCSAutoScrptz.sh
```

- **OCS Panel & VPS**
```
wget https://raw.githubusercontent.com/ZENON-VPN/ocs-panel/master/VPSnOCScrptZ.sh && chmod +x VPSnOCScrptZ.sh && ./VPSnOCScrptZ.sh
```

- **VPS Only (For Servers)** 
```
wget https://raw.githubusercontent.com/ZENON-VPN/ocs-panel/master/VPScrptZ.sh && chmod +x VPScrptZ.sh && ./VPScrptZ.sh
```

- **Disable Change Password in Panel**
```
wget https://raw.githubusercontent.com/ZENON-VPN/ocs-panel/master/DsblChngPW.sh && chmod +x DsblChngPW.sh && ./DsblChngPW.sh
```

- **Updates : Kill Multilogin, Delete All Expired Users**
```
cd && wget -O ClrkzOCSUpdate "https://raw.githubusercontent.com/ZENON-VPN/ocs-panel/master/update-ocs.sh" && chmod +x ClrkzOCSUpdate && sed -i -e 's/\r$//' ClrkzOCSUpdate && ./ClrkzOCSUpdate && rm ClrkzOCSUpdate
```

__________________________________________________
**NOTE**

 -ZENON-VPM.ML-
 
 **TimeZone**   :  Thailand
___________________________________________________
