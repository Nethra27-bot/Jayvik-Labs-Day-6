# Jayvik-Labs-Day-6

## Part A: IPv4 Theory (10 Marks)

**1. What is IPv4?**
IPv4 stands for Internet Protocol Version 4. It is a network-layer protocol used to identify devices and route data packets between networks.

**2. How many bits are in an IPv4 address?**
An IPv4 address contains 32 bits.

**3. What is an octet?**
An octet is a group of 8 bits. Its decimal value ranges from 0 to 255.

**4. How many octets are in an IPv4 address?**
An IPv4 address contains four octets separated by dots. Example: `192.168.1.10`.

**5. What is a subnet mask?**
A subnet mask identifies the network portion and host portion of an IPv4 address. Example: `255.255.255.0`.

**6. Difference between network portion and host portion?**
- Network portion: identifies the network or subnet.
- Host portion: identifies an individual device interface within that subnet.

**7. What is a private IPv4 address?**
A private IPv4 address is used within local networks, such as home, college, and office networks. It is not directly routable over the public internet.

**8. Write all three private IPv4 ranges.**

| Private IPv4 range | CIDR notation |
|---|---|
| 10.0.0.0 – 10.255.255.255 | `10.0.0.0/8` |
| 172.16.0.0 – 172.31.255.255 | `172.16.0.0/12` |
| 192.168.0.0 – 192.168.255.255 | `192.168.0.0/16` |

**9. What is a public IPv4 address?**
A public IPv4 address is an address that can be routed across the internet, subject to internet routing policies and address allocation rules.

**10. What is the IPv4 loopback address?**
`127.0.0.1` is the commonly used IPv4 loopback address. It allows a computer to send network traffic back to itself for testing.

**11. What is APIPA?**
APIPA stands for Automatic Private IP Addressing. Windows may automatically assign an address from `169.254.0.0/16` when it cannot obtain a usable IPv4 address from a DHCP server.

**12. What does 169.254.x.x commonly indicate?**
It commonly indicates that a device has assigned itself an APIPA address because it did not receive a usable IPv4 address through DHCP.

**13. What is a default gateway?**
A default gateway is usually a router that forwards traffic from a local network to destinations outside that network.

**14. Static vs dynamic IP addressing?**
- Static IP addressing: an IP address is configured manually or reserved to remain consistent.
- Dynamic IP addressing: an IP address is assigned automatically, usually by DHCP, and may change over time.

**15. What is DHCP?**
DHCP stands for Dynamic Host Configuration Protocol. It automatically assigns network settings, such as an IP address, subnet mask, default gateway, and DNS server addresses.

**16. What is a network address?**
A network address identifies a particular IPv4 subnet. In a conventional IPv4 subnet, all host bits are set to zero in the network address.

**17. What is a broadcast address?**
A broadcast address is used to send a packet to all hosts on a particular IPv4 subnet. In a conventional IPv4 subnet, all host bits are set to one in the broadcast address.

**18. Why is IPv4 knowledge important in cybersecurity?**
IPv4 knowledge helps cybersecurity professionals identify network devices, perform network mapping, understand subnetting, analyze network traffic, configure firewalls, troubleshoot connectivity, and investigate suspicious network activity.

---

## Part B: Practical Identification (4 Marks)

> ⚠️ The screenshots below show the Ethernet adapters only (`Ethernet` – disconnected, and `Ethernet 2`, a VirtualBox Host-Only adapter). The active Wi-Fi adapter's section of `ipconfig /all` wasn't captured, so those values are left blank. Re-run `ipconfig /all` and scroll to the Wi-Fi adapter section to fill them in.

| Required detail | Result |
|---|---|
| IPv4 address | `192.168.56.1` *(Ethernet 2 – VirtualBox Host-Only adapter)* |
| Subnet mask | `255.255.255.0` |
| Default gateway | Not assigned — host-only adapters have no internet gateway |
| DNS server(s) | Not shown for this adapter in the captured screenshot |
| DHCP status | Disabled |

**Wi-Fi adapter (connected, used for internet access):** fill in once you have its full `ipconfig /all` section.

---

## Part C: Screenshots (3 Marks)

### Screenshot 1 — `ipconfig`
*Not included — add a screenshot of the plain `ipconfig` output and save it as `screenshots/ipconfig_basic.jpg`.*

### Screenshot 2 — `ipconfig /all`
![ipconfig /all output](screenshots/ipconfig_all.jpg)

### Screenshot 3 — `ping 127.0.0.1`
![ping 127.0.0.1 output](screenshots/ping_loopback.jpg)

Confirms local TCP/IP loopback functionality: 4 packets sent, 4 received, 0% loss, round-trip time < 1 ms.

---

## Part D: Report Quality (3 Marks)

- [x] Name Nethra M and Day 06 appear at the top.
- [x] All 18 theory questions are answered.
- [ ] Practical details are filled in from the connected adapter (Wi-Fi row pending).
- [ ] All three screenshots are attached (`ipconfig` screenshot still needed).
- [x] Formatting and spelling checked.

---

## Conclusion

This assignment helped me understand IPv4 addressing, subnet masks, private and public IP ranges, APIPA, loopback addresses, default gateways, and DHCP. By practicing `ipconfig`, `ipconfig /all`, and `ping 127.0.0.1`, I learned how to inspect network configuration and test local TCP/IP functionality. These concepts provide a foundation for network troubleshooting and cybersecurity.
