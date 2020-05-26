# Shodan Dorks
*Dorks for shodan.io* website. Taken from publicly available sources.

# Shodan
_Shodan is a search engine that lets the user find specific types
of computers (webcams, routers, servers, etc.) connected to the internet using a variety of filters._

## Basic Shodan Filters
### city:
Find devices in a particular city.<br/>
`city:"Bangalore"`

### country:
Find devices in a particular country.<br/>
`country:"IN"`

### geo:
Find devices by giving geographical coordinates.<br/>
`geo:"56.913055,118.250862"`

### hostname:
Find devices matching the hostname.<br/>
`server: "gws" hostname:"google"`

### net:
Find devices based on an IP address or /x CIDR.<br/>
`net:210.214.0.0/16`

### os:
Find devices based on operating system.<br/>
`os:"windows 7"`

### port:
Find devices based on open ports.<br/>
`proftpd port:21`

### before/after:
Find devices before or after between a given time.<br/>
`apache after:22/02/2009 before:14/3/2010`

### Citrix:
Find Citrix Gateway.<br/>
`title:"citrix gateway"`

### Wifi Passwords:
Helps to find the cleartext wifi passwords in Shodan.</br>
`html:"def_wirelesspassword"`

### Surveillance Cams:
With username:admin and password: :P</br>
`NETSurveillance uc-httpd`

### Fuel Pumps connected to internet:
No auth required to access CLI terminal.</br>
`"privileged command" GET`

### Windows RDP Password:
But may contain secondary windows auth</br>
`"\x03\x00\x00\x0b\x06\xd0\x00\x00\x124\x00"`

### Mongo DB servers:
It may give info about mongo db servers and dashboard </br>
`"MongoDB Server Information" port:27017 -authentication`

### FTP servers allowing anonymous access:
Complete Anon access </br>
`"220" "230 Login successful." port:21`

### Jenkins:
Jenkins Unrestricted Dashboard </br>
`x-jenkins 200`

### Hacked routers:
Routers which got compromised </br>
`hacked-router-help-sos`

### Open ATM:
May allow for ATM Access availability </br>
`NCR Port:"161"`

### Telnet Access:
NO password required for telnet access. </br>
`port:23 console gateway`

### Misconfigured Wordpress Sites:
The wp-config.php if accessed can give out the database credentials. </br>
`http.html:"* The wp-config.php creation script uses this file"`

### Hiring:
Find sites hiring. </br>
`"X-Recruiting:"`

### Android Root Bridge:
Find android root bridges with port 5555. </br>
`"Android Debug Bridge" "Device" port:5555`

### Etherium Miners:
Shows the miners running ETH. </br>
`"ETH - Total speed"`

### Tesla Powerpack charging Status:
Helps to find the charging status of tesla powerpack. </br>
`http.title:"Tesla PowerPack System" http.component:"d3" -ga3ca4f2`




### YOU CAN ALSO COMBINE FILTERS TO MAKE INTO ADVANCED FILTERS FOR QUICK RECON.

*Please create a pull request if you want to contribute.*
