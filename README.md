# Elevate_Labs-CybersecurityInternship-TASK-1
# 🌐 Nmap Network Scanning Report

## 📌 Objective
Perform a network scan on the local subnet using **Nmap** to identify active hosts and discover open TCP ports.

---

## 🛠️ Tools Used
- 🐧 Kali Linux
- 🔍 Nmap 7.98
- 💻 Terminal

---

## 📍 Network Information

| Item | Value |
|------|-------|
| 🌐 Local IP | 192.168.31.52 |
| 📡 Network Range | 192.168.31.0/24 |
| 🖥️ Interface | eth0 |

---

## 🚀 Commands Used

### 1️⃣ Check IP Address
```bash
ip addr
```

### 2️⃣ Discover Live Hosts
```bash
nmap -sn 192.168.31.0/24
```

### 3️⃣ Perform TCP SYN Scan
```bash
nmap -sS -oN result_tcp.txt 192.168.31.0/24
```

### 4️⃣ View Scan Result
```bash
cat result_tcp.txt
```

---

## 📊 Scan Results

### ✅ Active Hosts Found
- 📍 192.168.31.1 (JioFiber Router)
- 📍 192.168.31.52 (Kali Linux)
- 📍 192.168.31.141 (Desktop)
- 📍 192.168.31.179 (Android Device)

---

## 🔓 Open Ports Found (Router)

| Port | Service | Status |
|------|---------|--------|
| 53 | DNS | ✅ Open |
| 80 | HTTP | ✅ Open |
| 443 | HTTPS | ✅ Open |
| 7443 | Oracle HTTPS | ✅ Open |
| 8080 | HTTP Proxy | ✅ Open |
| 8443 | HTTPS Alt | ✅ Open |

---

## 🔍 Observations

✔️ Total Hosts Detected: **4**

✔️ Router has multiple management and web service ports open.

✔️ Desktop and Android device did not expose open TCP ports.

✔️ Kali Linux successfully communicated with all active devices.

---

## 🎯 Conclusion

The network scan was successfully completed using **Nmap**.

The scan identified active devices in the local network and detected open TCP ports on the router. This exercise demonstrated how Nmap can be used for host discovery and basic network reconnaissance.

---

## 📂 Output File

```
result_tcp.txt
```

---

## ✅ Status

**Task Completed Successfully** ✔️