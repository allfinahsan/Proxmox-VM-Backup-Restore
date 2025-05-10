# 🧪 Proxmox VM Backup + Restore Lab

This project documents how I backed up and restored virtual machines using **Proxmox Backup Server (PBS)** inside a VLAN-isolated network environment. Everything is tested in my homelab using real hardware and a custom network layout (VLAN 86).

---

## 🌐 Environment
- Proxmox VE 8
- Proxmox Backup Server 3.4
- VLAN 86 (dedicated backup network)
- External HDD as datastore

---

## 🎯 Objectives
- Perform **daily full backups** for all VMs to PBS
- Automate snapshot jobs with custom retention policy
- Simulate VM restore to a secondary node
- Validate restore with both GUI + CLI methods

---

## 📂 Folder Structure

| Folder/File             | Purpose                                        |
|-------------------------|------------------------------------------------|
| `/screenshots/`         | Interface + process screenshots                |
| `/configs/`             | PBS backup config (`vm-id: all`), network setup |
| `restore-guide.md`      | Step-by-step CLI + GUI restore instructions    |
| `project-summary.md`    | Non-technical summary and goals                |

---

## 🧠 Learnings
- How to back up **all VMs** automatically using `vm-id: all`
- Benefits of VLAN isolation for backup traffic
- Backup rotation (daily/weekly/monthly) with `zstd` compression
- CLI vs GUI recovery workflows and when to use each

---

## 📌 Next Steps
- Automate backup job monitoring with shell script or alert
- Sync offsite backups to cloud via `rclone` or `S3`
- Integrate Grafana for storage and backup job metrics

---

## 📸 Screenshots

### 🖥️ Proxmox Dashboard (VM Overview)
![Proxmox Dashboard](./screenshots/proxmox-dashboard.png)

### 💾 PBS Backup Server (Job Status)
![PBS Dashboard](./screenshots/pbs-dashboard.png)

---
