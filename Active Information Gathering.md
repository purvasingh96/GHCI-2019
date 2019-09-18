# Active Information Gathering

# Software Installation

To play-around with active information gathering concepts, [Metasploitable2](https://sourceforge.net/projects/metasploitable/) is the best option to go with.<br>
**Metasploitable** is intentionally vulnerable VM, which emulates a vulnerable target and is used to practice common penetration methods.

# NMap

* NMap or network-mapper is free and open source tool used for *vulnerability scanning and discovery.*
* Identifies devices that are running on your local network.
* It scans multiple hosts
* Nmap work by sending raw packets to system hosts. By doing this it listens to responses and determines whether ports are open or close.
* Nmap also detect OS running on web you are scanning and detects vulnerabilities.


| S.No | N-Map commands             | Description                |
|------|----------------------------|----------------------------|
| 1.   | `nmap <your-ip-address>`     | Scan a single IP           |
| 2.   | `nmap -A <your-ip-address>`  | Detect OS and Services     |
| 3.   | `nmap -sV <your-ip-address>` | Standard service detection |
| 4.   | `nmap -sT 192.168.1.1`       | Scan using TCP connect. Performs full 3-way handshake inorder to scan target.     |
| 5.   | `nmap -sS 192.168.1.1`     | Scan using TCP SYN scan (default) |
| 6.   | `nmap -Pn 192.168.1.19`     | Discovers open ports. |


# By-pass Firewalls with Nmap

* *ACK signal* can be used to bypass some of the rules of router.
* If there is a rule that allows SYN-packets only from inter-network (machines that are on target machine's local network), and a 3-way handshake rule is enabled, you can trick the target PC by sending only *ACK signal*, which would make PC think it is a response to previous SYN-ACK bit.
* Whenever N-Map sends packets and if target PC knows that N-Map exists, they can make a rule that blocks any packets of standard N-Map size.

| S.No | N-Map commands                        | Description                                             |
|------|---------------------------------------|---------------------------------------------------------|
| 1.   | `nmap -sA <your-ip-address>`            | Use when there is a blockage  of SYN bit-set on target  |
| 2.   | `nmap --data -length <your-ip-address>` | Detect standard length of N-Map's packet size           |

# Spoofing MAC Address using Nmap

* *White-listing IP-addresses* means that the target PC has *allowed* list of certain IP-addresses to pass through.
* *Black-listing IP addresses* means that the target PC has *blocked* list of certain IP-addresses to pass through.
* Type in the following commands to spoof your MAC address with white-listed IP-address.
```
root@kali: nmap -g 80 <your-IP-address>
nmap --spoof --mac <sppof-MAC-address> <your-IP-address>
```

# Advanced Nmap Scripts
* Nmap scripts can be found in this location : `cd /usr/share/nmap/scripts`.
* Clone the following repository : [VulScan](https://github.com/scipag/vulscan)
* Following commands *rates a website* based on vulnerability on a scale of 1-10.
```
root@kali: nmap --script=ssh-brute.nse <your-IP-address>
nmap --script vulscan, nmap-vulners -sV <your-IP-address>

```
