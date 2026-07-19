# 08 - Network Commands 

## Objective

In this chapter, I learned the basic Linux networking commands used to check network configuration, test connectivity, identify the device, view routing information, inspect network connections, communicate with web servers, and download files.

---

## Commands Learned

### ip addr

Displays detailed information about network interfaces, including IPv4, IPv6, MAC Address, and interface status.

Example:

ip addr
---

### ping

Tests connectivity between the local machine and another host.

Example:

ping google.com
---

### hostname

Displays the hostname of the current machine.

Example:

hostname
---

### hostname -I

Displays the IPv4 address of the current machine.

Example:

hostname -I
---

### ip route

Displays the routing table and the default gateway.

Example:

ip route
---

### ss

Displays active network connections and sockets.

Example:

ss
---

### curl

Sends a request to a web server and displays the response in the terminal.

Example:

curl https://example.com
---

### wget

Downloads files from the internet.

Example:

wget https://example.com/file.zip
---

## Practice

- Used ip addr to display network interface information.
- Identified the IPv4 address of the machine.
- Checked whether the network interface was UP.
- Used hostname to display the machine name.
- Used hostname -I to quickly display the machine IPv4 address.
- Tested network connectivity using:

ping google.com
- Learned how to stop ping using:

Ctrl + C
- Viewed the routing table using:

ip route
- Identified the Default Gateway.
- Displayed active network connections using:

ss
- Sent a request to a web server using:

curl https://example.com
- Downloaded a file using:

wget https://example.com/file.zip
---

## What I Learned

- The difference between ip addr and hostname -I.
- The difference between hostname and hostname -I.
- How to test connectivity using ping.
- Why ping to an IP address can succeed while ping to a domain name can fail because of DNS issues.
- How to identify the Default Gateway using ip route.
- The purpose of ss for viewing active network connections.
- The difference between curl and wget.
- When to use curl and when to use wget.

---

## Notes

- ip addr displays complete network interface information.
- hostname displays the device name.
- hostname -I quickly displays the IPv4 address.
- UP means the network interface is enabled.
- ping checks connectivity but cannot identify every network problem.
- Ctrl + C stops the running ping process.
- default in ip route represents the Default Gateway.
- ss displays active network connections.
- ESTAB means the connection is established.
- curl is commonly used to communicate with web servers and APIs.
- wget is mainly used to download files.
