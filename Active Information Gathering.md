# Active Information Gathering

# Software Installation

To play-around with active information gathering concepts, [Metasploitable2](https://sourceforge.net/projects/metasploitable/) is the best option to go with.<br>
**Metasploitable** is intentionally vulnerable VM, which emulates a vulnerable target and is used to practice common penetration methods.

# N-Maps

* N-Maps or netwrok-mapper is free and open source tool used for *vulnerability scanning and discovery.*
* Identifies devices that are running on your local network.
* It scans multiple hosts
* N-Maps work by sending raw packets to system hosts. By doing this it listens to responses and determines whether ports are open or close.
* N-Maps also detect OS running on web you are scanning and detects vulnerabilities.


| S.No | N-Map commands             | Description                |
|------|----------------------------|----------------------------|
| 1.   | `nmap <your-ip-address>`     | Scan a single IP           |
| 2.   | `nmap -A <your-ip-address>`  | Detect OS and Services     |
| 3.   | `nmap -sV <your-ip-address>` | Standard service detection |
| 4.   | `nmap -sT 192.168.1.1`       | Scan using TCP connect     |
| 5.   | `nmap -sS 192.168.1.1`     | Scan using TCP SYN scan (default) |
