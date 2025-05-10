# 🔄 VM Restore Guide – Proxmox + PBS

## GUI Method

1. Login to Proxmox Web UI
2. Navigate to the PBS storage
3. Select the VM ID → Backup → Choose snapshot
4. Click **Restore**
   - Target node: select current or secondary node
   - Choose "Unique MAC address" to avoid conflicts
   - Keep original VM ID or assign new
5. Wait for job completion
6. Start the VM and test services

---

