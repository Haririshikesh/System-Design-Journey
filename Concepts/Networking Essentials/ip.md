# IP (Internet Protocol)

> **“Just like your house needs an address to receive letters, your device needs an IP address to receive data from the internet.”**

---

## What is an IP Address?

An **IP address** is a unique number assigned to every device connected to the internet. It helps in:

Identifying the device  
Finding its location in the network  
Sending and receiving data between devices

> **Simple analogy**: Your phone, laptop, or smart TV is like a house in a massive digital city (the Internet). IP is its address. Without it, data won’t know where to go.

---

## Versions of IP

### 1. IPv4 (Internet Protocol version 4)

**Format**: 4 sets of numbers separated by dots (e.g., 192.168.0.1)  
**Total Addresses**: ~4.3 billion  
**Example**: 102.22.192.181

> Still widely used but running out of addresses due to internet growth.

### 2. IPv6 (Internet Protocol version 6)

**Format**: 8 groups of alphanumeric characters (e.g., 2001:0db8:85a3::8a2e:0370:7334)  
**Total Addresses**: 340 trillion trillion trillion (massive!)  
**Example**: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

> Solves the address shortage problem. Slowly replacing IPv4.

---

## Types of IP Addresses

### 1. Public IP

Given by your **Internet Service Provider (ISP)** to your **home network (router)**
This is how the world sees your network
**Same public IP** is used by all devices in your home to connect to the internet

**Example:**  
You Google "weather" from your phone, and Google sends the data to your public IP: 103.45.22.11. Your router then sends it to your phone.

---

### 2. Private IP

Assigned **inside your local network** to each device (like phone, laptop, smart TV)
Not visible on the internet
Used for **device-to-device communication** within your home or office

**Example:**  
Your laptop’s private IP might be 192.168.0.5, while your phone’s is 192.168.0.6. These are assigned by your router automatically.

---

### 3. Dynamic IP (Most Common)

Automatically assigned by a **DHCP server** (usually your Wi-Fi router)
**DHCP** = Dynamic Host Configuration Protocol
It assigns IPs temporarily to devices
IP address can change if you disconnect and reconnect

**Example:**  
Today your public IP is 103.45.22.11. Tomorrow, it might be 103.45.22.19. You didn’t do anything—your ISP rotated it.

**Why it’s used?**
Easy to manage  
Saves IP address space  
Cheaper for ISPs

---

### 4. Static IP

Manually assigned and doesn’t change  
Used when **consistent reachability** is needed (like for websites or servers)

**Example (Practical):**  
You host your own website on a server at home. You want people to access it via the same IP every time.  
Your static IP might be: 49.206.45.117.

**Use cases:**  
Hosting a website or game server  
CCTV camera systems with remote access  
Remote work (connecting to office servers)

---

## Let’s Visualize With a Real-Life Scenario

**You open YouTube on your phone at home. What happens?**

![IPExample](/ReferenceImages/ip_example.jpg)

This is how the request passes and reaches the server . Then the response will be sent back to you in the backward flow.

---

## How to Check Your IP

**Public IP:** Google “What is my IP?”

**Private IP:**

* **Windows:** Open **Command Prompt** and type `ipconfig`. Look for the "IPv4 Address" under your active network adapter (e.g., "Wi-Fi" or "Ethernet").
* **Mac/Linux:** Open **Terminal** and type `ifconfig` or `ip a`. Look for the "inet" address under your active network interface (e.g., "wlan0" for Wi-Fi or "eth0" for Ethernet).


## For More Reference => [Resources](/Resources/)
