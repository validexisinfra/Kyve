# Kyve
KYVE, the Web3 data lake solution, is a protocol that enables data providers to standardize, validate, and permanently store blockchain data streams.

# 🌟 Kyve Setup & Upgrade Scripts

A collection of automated scripts for setting up and upgrading Kyve nodes on **Mainnet (`kyve-1`)**.

---

### ⚙️ Validator Node Setup  
Install a Kyve validator node with custom ports, snapshot download, and systemd service configuration.

~~~bash
source <(curl -s https://raw.githubusercontent.com/validexisinfra/Kyve/main/installmain.sh)
~~~
---

### 🔄 Validator Node Upgrade 
Upgrade your Kyve node binary and safely restart the systemd service.

~~~bash
source <(curl -s https://raw.githubusercontent.com/validexisinfra/Kyve/main/upgrademain.sh)
~~~

---

### 🧰 Useful Commands

| Task            | Command                                 |
|-----------------|------------------------------------------|
| View logs       | `journalctl -u kyved -f -o cat`        |
| Check status    | `systemctl status kyved`              |
| Restart service | `systemctl restart kyved`             |
