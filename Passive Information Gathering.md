# Passive Information Gathering

# Google Hacking
* finds all sites that require user input vulnerable to SQL injection
* Visit **[Google Hacking Database](https://www.exploit-db.com/google-hacking-database)** for more SQL queries.


| S.No | Google Hacking Commands        | Output                                                                             |
|------|-------------------------------|------------------------------------------------------------------------------------|
| 1.   | `inurl : "index.php?id="`       | finds out links that ends with "index.php?id="; <br>e.g https://www.atmarine.fi/?id=2  |
| 2.   | `inurl:"/fuel/login"`           | Pages containing login pages;<br> http://lcp.loctell.com/dy-fuel/login                 |
| 3.   | `inurl:users.json + "username"` | Pages containing password;<br> https://github.com/get/homeslice/blob/master/users.json |
