# Passive Information Gathering

# Google Hacking
* finds all sites that require user input vulnerable to SQL injection
* Visit **[Google Hacking Database](https://www.exploit-db.com/google-hacking-database)** for more SQL queries.


| S.No | Google Hacking Commands        | Output                                                                             |
|------|-------------------------------|------------------------------------------------------------------------------------|
| 1.   | `inurl : "index.php?id="`       | finds out links that ends with "index.php?id="; <br>e.g https://www.atmarine.fi/?id=2  |
| 2.   | `inurl:"/fuel/login"`           | Pages containing login pages;<br> http://lcp.loctell.com/dy-fuel/login                 |
| 3.   | `inurl:users.json + "username"` | Pages containing password;<br> https://github.com/get/homeslice/blob/master/users.json |


# Nikto Basics

* [Nikto](https://hackertarget.com/nikto-website-scanner/) is a popular web scanner software.
* This testing service can be used to test a Web Site, Virtual Host and Web Server for known security vulnerabilities and mis-configurations.
* Below is a command to scan a particular IP-address -<br>
```
run nikto
provide <target-host/IP-address>
nikto -h <target-host/IP-address> 
```
# EmailHarvester
* [EmailHarvester](https://github.com/maldevel/EmailHarvester) tool to retrieve Domain email addresses from Search Engines.

| S.No | EmailHarvester commands                                  | Description                                  |
|------|----------------------------------------------------------|----------------------------------------------|
| 1.   | `./EmailHarvester.py -d example.com -e google `            | Search in Google                             |
| 2.   | `./EmailHarvester.py -d example.com -e googleplus`         | Search in site using Search engines          |
| 3.   | `./EmailHarvester.py -d example.com -e all -r twitter,ask` | Search in all engines/sites but exclude some |
