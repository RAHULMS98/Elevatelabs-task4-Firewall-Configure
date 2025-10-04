# 🔥 Firewall Configuration on Windows

## 🎯 Objective
To configure and test basic firewall rules on **Windows Defender Firewall** to block and verify network traffic on **port 23 (Telnet)**.  
This exercise demonstrates essential firewall management skills such as creating, testing, and removing rules for system security.

---

## 🧰 Tools Used
- **Windows Defender Firewall**
- **Telnet Client (Command Prompt)**

---

## ⚙️ Implementation Steps

### 1. **Firewall Status Check**
Opened **Windows Defender Firewall** and confirmed it was enabled for **Private**, **Public**, and **Domain** profiles.  
The default configuration was:
- **Inbound connections:** Blocked unless explicitly allowed  
- **Outbound connections:** Allowed unless explicitly blocked  

---

### 2. **Rule Creation**
Created a new **Inbound Rule** using the *New Rule Wizard* under *Advanced Settings*.

| Setting | Configuration |
|----------|----------------|
| Rule Type | Port |
| Protocol | TCP |
| Port | 23 (Telnet) |
| Action | Block the connection |

---

### 3. **Testing the Block**
Tested the rule using the **Telnet Client** in Command Prompt:
```bash
telnet localhost 23
Could not open connection to the host, on port 23: Connect failed
