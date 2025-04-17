# 🌐 IP Addressing

Each and every device needs the IP address for communication.

## 🔢 Types: => 2
1. **IPv4** ➡️ 16 characters with 4 divisions separated by ":"  
   📍 *Start Range:* `0.0.0.0`  
   📍 *End Range:* `255.255.255.255`  
   📌 *(e.g., short phoneNumber)*

2. **IPv6** ➡️ 24 characters with 6 divisions separated by ":"

---

## 📡 IPv4 
👉 Use `ping` command to find the IP of a particular URL  
📌 Example: `ping www.google.com`  
🔍 *This will return an IP address like:* `142.250.195.36`

---

## 🗂️ Classes: A B C D E  
💡 **Hint:** "1st address and last address for host named as Broadcast"

### 🅰️ Class A  
- Range: `1.0.0.0` to `126.255.255.255`  
- Usage: **Large Networks**  
- 📍 `127.x.x.x` is **Loopback Address** → it pings its own device  
  📌 Example: `ping 127.0.0.1`

### 🅱️ Class B  
- Range: `128.0.0.0` to `191.255.255.255`  
- Usage: **Medium Networks**

### 🌐 Class C  
- Range: `192.0.0.0` to `223.255.255.255`  
- Usage: **Local Area Networks (LAN)**

### 🛰️ Class D  
- Range: `224.0.0.0` to `239.255.255.255`  
- Reserved for **Multicasting**

### 🧪 Class E  
- Range: `240.0.0.0` to `255.255.255.254`  
- Reserved for **Experimental purposes**

💡 *Classes A, B, and C depend on the size and requirements of the network.*

---

## 💰 AWS Charging Note
AWS is charging for IPv4 because at some point it may become **exhausted**.  
📘 So, **RFC1918** came up with a formula → **Private and Public IPs**

---

## 🔐 Private IPs (Used in office environments)

🛜 These are used internally and translated to Public IPs for external communication.

- `10.0.0.0` - `10.255.255.255` (🔑 10/8 prefix)  
- `172.16.0.0` - `172.31.255.255` (🔑 172.16/12 prefix)  
- `192.168.0.0` - `192.168.225.255` (🔑 192.168/16 prefix)

📌 Example in Offices:  
A router may assign `192.168.1.2` to your laptop.

📌 Example in AWS EC2:  
You might see `10.0.1.15` as the private IP of an instance.

---

