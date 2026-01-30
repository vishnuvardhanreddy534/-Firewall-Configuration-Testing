# Task 10: Firewall Configuration & Testing

## 📌 Objective
The objective of this task is to understand firewall concepts and gain hands-on experience in configuring and testing firewall rules using UFW / Windows Firewall. This task focuses on controlling network traffic, improving system security, and documenting firewall rules and their impact.

---

## 🧠 Firewall Concepts
A firewall is a security mechanism that monitors and controls incoming and outgoing network traffic based on predefined rules. It acts as a barrier between trusted internal systems and untrusted external networks.

---

## 🛠 Tools Used
- **Primary Tools:**  
  - UFW (Uncomplicated Firewall)  
  - Windows Firewall  

- **Alternative Tool:**  
  - iptables  

---

## ⚙️ Firewall Configuration Steps

### 1️⃣ Enable Firewall
- Firewall enabled with a default policy of denying incoming traffic and allowing outgoing traffic.

### 2️⃣ Configure Firewall Rules
Firewall rules were created to allow required services and block insecure or unused ports.

| Rule | Action | Port / IP | Purpose |
|-----|-------|-----------|--------|
| Allow | Inbound | 22 (SSH) | Secure remote access |
| Allow | Inbound | 80 (HTTP) | Web traffic |
| Allow | Inbound | 443 (HTTPS) | Secure web traffic |
| Deny | Inbound | 21 (FTP) | Block insecure service |
| Deny | Inbound | 23 (Telnet) | Block legacy protocol |
| Deny | Inbound | Malicious IP | Prevent suspicious activity |

---

## 🚦 Allow / Deny Ports
- **Allowed Ports:** SSH (22), HTTP (80), HTTPS (443)
- **Blocked Ports:** FTP (21), Telnet (23)

Blocking unused and insecure ports helps reduce the system’s attack surface.

---

## 🔍 Connectivity Testing
Connectivity was tested using:
- `ping` for reachability
- Port scanning tools to verify open and blocked ports
- Browser testing for HTTP/HTTPS access

✔ Allowed ports were accessible  
✖ Blocked ports were filtered or denied

---

## 📜 Firewall Logs
Firewall logging was enabled to monitor traffic.

### Observed Log Details:
- Source IP address
- Destination port
- Protocol
- Action taken (ALLOW / DENY)
- Timestamp

Logs help in detecting suspicious behavior and support incident investigation.

---

## 🚫 Blocking Malicious IP
A suspicious IP showing repeated unauthorized access attempts was identified from firewall logs and blocked using a deny rule.

### Result:
- Unauthorized attempts stopped
- System security improved

---

## 📊 Impact Analysis

### Positive Impact
- Reduced attack surface
- Protection against unauthorized access
- Improved visibility into network traffic
- Better system hardening

### Risks of Misconfiguration
- Blocking legitimate services
- Network connectivity issues
- Potential downtime

---

## ✅ Final Outcome
- Hands-on firewall configuration experience
- Understanding of network traffic filtering
- Practical firewall management skills
- Readiness for real-world SOC and system administration roles

---

## 📂 Repository Contents
- Firewall Configuration Report (PDF)
- Firewall Screenshots (JPG)
- README.md

---

## 👤 Author
**T VISHNU VARDHAN REDDY**
