# Wireless Penetration Testing via De-authentication Frames

## Pre-requisites
Enable **monitor mode** for your network adapter. You can use the following commands to enable monitor mode - 
```
sudo ifconfig wlan0 down
sudo iwconfig wlan0 mode monitor
sudo ifconfig wlan0 up
```
<img src="./images/step-1-enable-monitor-mode.png"></img>

# Steps to perform de-authentication attack

## Step-1: Check Interfering Process 
`airmon-ng` can be used to check the process currently running that **can interfere and prevent us** from performing our wireless penetration attack.<br>
Command used to check the interfering process is -<br>
```
sudo airmon-ng start wlan0
```
<img src="./images/step-2-check-interfering-process.png"></img>

## Step-2: Kill Interfering Process 
`airmon-ng` again can be used to kill the interfering processes discovered in step-1.<br>
Command used to kill the interfering process is -<br>
```
sudo airmon-ng check kill wlan0
```
<img src="./images/step-3-kill-interferring-process.png"></img>
