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

# Shodan Search Engine

[Shodan](https://www.shodan.io/) is a search engine that lets user find specific types of computers connected to internet using variety of filters.

# DNS Zone transfers with Dig

* Dig command reads the /etc/resolv.conf file and querying the DNS servers listed there. The response from the DNS server is what dig displays.
* Using dig (domain information groper), attackers can make use of replication for primary and secondary DNS servers in order to be synchronized.
* From secondary server, attackers can ask for data from primary server.
* Primary server answers with copy of database which has IP-address and host names.
* If attackers get hold of all your DNS records, they can use those records to replicate DB across group of DNS servers
* **Sample commands** -<br>

| S.No | Dig commands         | Description                         |
|------|----------------------|-------------------------------------|
| 1.   | `dig yahoo.com +short` | Query Domain “A” Record with +short |
| 2.   | `dig yahoo.com MX`     | Querying MX Record for Domain       |
| 3.   | `dig yahoo.com SOA`    | Querying SOA Record for Domain      |
