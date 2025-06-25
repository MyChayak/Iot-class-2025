# 📄 Debian Installation Report for IoT, MQTT, Kafka Course

> Students must complete all sections of this form during Debian installation and submit it upon completion.

---

## 🔧 General Information

| Title                  | Value                                               |
| -----------------------| --------------------------------------------------- |
| Full Name              | Chayakarn Phuwavilaimetha|
| Student ID              | 6510301013 |
| Installation Date      | 11/06/2025 |


---

## 🖥️ Device Information

- 💻 **Device Model / Type**: Virtual Machine
- 🧬 **Firmware Type**:  
  - [ ] UEFI  
  - [x] BIOS  
- 🏷️ **Installation Type**:  
  - [ ] Physical PC  
  - [x] Virtual Machine (VM)

---

## 🗂️ Custom Partitioning

| Partition     | Size   | Filesystem | Mount Point           | Notes              |
|---------------|--------|------------|------------------------|--------------------|
| /dev/sda1     | 19G    | ext4       | /                      | Root filesystem    |
| udev          | 1.9G   | tmpfs      | /dev                   | Device files       |
| tmpfs         | 392M   | tmpfs      | /run                   | Runtime data       |
| tmpfs         | 2.0G   | tmpfs      | /dev/shm               | Shared memory      |
| tmpfs         | 5.0M   | tmpfs      | /run/lock              | Lock files         |
| tmpfs         | 392M   | tmpfs      | /run/user/1000         | User runtime files |


---

## 🌐 Network Configuration (Static IP)

| Title                   | Value                                               |
| ------------------------| --------------------------------------------------- |
| Network Interface Name  | ens18     |
| IP Address              | 172.30.15.29 |
| Netmask                 | 255.255.255.0 |
| Gateway                 | 172.30.15.254 |
| DNS                     | 172.30.15.254 , 8.8.8.8 |

---

## 🖧 Hostname

- 🖥️ **Hostname Set**: FDT6510301013

---

## 👤 User Account

- 👨‍💻 **Username Created**: u6510301013
- 🔐 **Is a Root Password Set?**:  
  - [X] Yes  
  - [ ] No

---

## ✅ Additional Problems Notes (if any)

> _____________________________________________________________________  
> _____________________________________________________________________  
> _____________________________________________________________________

