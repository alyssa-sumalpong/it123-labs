# Lab Notes – Week 2  
_First Graded Lab Assessment_  

---

# VM Creation – Windows Server 2019  
- Opened Oracle VirtualBox → Clicked "New"
- VM Name: Windows_Server
- Machine Folder: `it123-labs/VMs/`  
- Type: Microsoft Windows  
- Version: Windows Server 2019 (64-bit)
- Memory: 4069 MB (4 GB)
- CPU: 1 core  
- Virtual Hard Disk: 50 GB, VDI, dynamically allocated
- Attached ISO: Windows Server 2019 Evaluation ISO  

---

# Installation Steps – Windows  
1. Started VM with ISO mounted.  
2. Windows Setup → Language: English (United States).  
3. Clicked 'Install Now'.  
4. Selected 'Windows Server 2019 Standard Evaluation (Desktop Experience)'  
5. Accepted License Agreement.  
6. Selected Custom: Install Windows only (advanced)  
7. Deleted old partitions → Chose 'Unlocated Space'.
8. Installation started (Copying files, Installing features, etc.).  
9. After reboot → Set up the required Administrator password.  
10. Entered password: 'Passw0rd123'
11. Logged in as 'admin' for the first time.

---

# Post-Installation Config – Windows  
- Network Adapter 1: 'NAT' (default, internet access).  
- (Optional) Network Adapter 2: **Host-Only** (for private LAN later).  
- Took **Snapshot**: “Clean Install – Windows Server”.  

---

# VM Creation – Ubuntu Server 22.04  
- Opened Oracle VirtualBox → Clicked 'New'
- VM Name: **UbuntuServer22-Lab**  
- Machine Folder: `it123-labs/VMs/`  
- Type: **Linux**  
- Version: **Ubuntu (64-bit)**  
- Memory: **2048 MB (2 GB)**  
- CPU: **2core**  
- Virtual Hard Disk: **30 GB, VDI, dynamically allocated**
- Attached ISO: **Ubuntu Server 22.04 LTS ISO**  

---

# Installation Steps – Ubuntu  
1. Started VM with ISO mounted.  
2. Selected Install Ubuntu Server.  
3. Language: English.  
4. Keyboard layout: English (US).  
5. Network: Accepted default (DHCP, NAT).  
6. Storage: Used Guided – Use Entire Disk (auto-partition).  
7. User setup:  
   - Username: **admin**  
   - Password: **P@ssw0rd123**  
8. Installation downloaded and installed the base system.  
9. Skipped optional snaps and featured server packages.  
10. Installation finished → Rebooted into the Ubuntu login screen.  
11. Logged in successfully with user **admin**.  

---

# Post-Installation Config – Ubuntu  
- Network Adapter 1: NAT (internet enabled by default).  
- Took **Snapshot**: “Clean Install – Ubuntu Server”.  

---

# Summary of VM Configurations  

| VM Name            | OS Version                       | RAM   | CPU | Storage | Network | Username | Password     | Snapshot                  |
|--------------------|----------------------------------|-------|-----|---------|---------|----------|--------------|---------------------------|
| WinServer2019-Lab  | Windows Server 2019 (Eval, GUI) | 4069 MB | 1   | 50 GB   | NAT     | admin    | P@ssw0rd123 | Clean Install – Windows   |
| UbuntuServer22-Lab | Ubuntu Server 22.04 LTS         | 2048 MB | 2   | 30 GB   | NAT     | admin    | P@ssw0rd123 | Clean Install – Ubuntu    |

---

# Issues Encountered  
- Windows: Password confirm button not clickable → Solved with **Tab + Enter**.  
- Windows: Warning about Windows.old → Fixed by deleting old partitions.  
- Ubuntu: Slower installation due to package updates (solved by waiting).  

---

#Conclusion  
Successfully created and installed two VMs (Windows Server 2019 and Ubuntu Server 22.04 LTS) in VirtualBox, configured system resources, enabled networking, and documented the process. Both are ready for use in future labs.  
