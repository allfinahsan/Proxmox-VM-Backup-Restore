# 🔍 Project Summary – Proxmox VM Backup & Restore

This homelab project demonstrates a full backup and disaster recovery workflow using **Proxmox VE 8** and **Proxmox Backup Server 3.4**, configured inside a **VLAN-isolated environment (VLAN 86)**.

---

## 💡 Why I Built This
To practice real-world backup automation, VM recovery, and secure traffic separation — all critical skills for infrastructure, DevOps, and cybersecurity roles.

---

## ✅ What I Did
- Backed up **all VMs** daily to a dedicated Proxmox Backup Server
- Created a **custom retention policy** for snapshots (daily/weekly/monthly)
- Verified backup health via PBS interface
- Restored test VMs using **GUI and CLI**
- Isolated backup traffic using **VLAN 86**

---

## 🧰 Tools + Tech Stack
- Proxmox VE 8 + PBS 3.4
- VLAN config on UDM SE
- External HDD datastore
- `zstd` compression + snapshot mode
- Manual + scheduled PBS jobs

---

## 📂 Project Files
- `restore-guide.md` – step-by-step recovery process
- `backup-job.conf` – PBS job config (`vm-id: all`)
- `/screenshots/` – interface walkthroughs
- `/configs/` – sample job and VLAN layout (coming)

---

## 🧠 Key Skills Demonstrated
- Infrastructure planning and execution
- Backup automation with enterprise-grade tools
- Network segmentation and traffic isolation
- Markdown documentation and GitHub repo structuring

---

📍 Live Repo: [Proxmox-VM-Backup-Restore on GitHub](https://github.com/allfinahsan/Proxmox-VM-Backup-Restore)
