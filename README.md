# 🔥 UFW Firewall Configuration – Parrot OS

## 🛡️ Objective
To configure and verify the firewall using UFW (Uncomplicated Firewall) on Parrot OS to:
- Enable firewall protection
- Allow incoming SSH (port 22)
- Block incoming Telnet (port 23)
- List and verify all rules
- Demonstrate how firewall rules filter traffic

---

## ⚙️ Commands Used

### 🔹 Enable UFW
```bash
sudo ufw enable
```

### 🔹 Allow SSH (Port 22)
```bash
sudo ufw allow 22
```

### 🔹 Deny Telnet (Port 23)
```bash
sudo ufw deny 23
```

### 🔹 Check Status with Rule Numbers
```bash
sudo ufw status numbered
```

---

## 🧪 Testing

- ✅ SSH on port 22 should be accessible:
  ```bash
  ssh localhost
  ```

- ❌ Telnet on port 23 should be blocked:
  ```bash
  telnet localhost 23
  ```

---

## 📸 Screenshots

- **Firewall Enabled**
- **Rules Applied: ALLOW 22 / DENY 23**

(Screenshots included in documentation folder)

---

## ✅ Summary

- UFW simplifies firewall rule creation on Linux systems.
- Rules can be added per port, IP, or protocol.
- Helps to secure services by explicitly defining access permissions.

---

## 📎 Notes

- Always allow port 22 before enabling UFW on remote systems to avoid being locked out.
- Telnet is an insecure protocol and should remain blocked in modern networks.
