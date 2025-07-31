# 🌐 Project Title  
**Cross-Region Backup & Restore of Azure VM using Azure Recovery Services Vault**

---

## 📌 Objective  
This project demonstrates how to configure backup for an Azure VM using Recovery Services Vault (RSV) and perform a **cross-region restore** to a different Azure region, ensuring **disaster recovery** and **business continuity**.

---

## 🧱 Tech Stack  

- ✅ Azure Virtual Machine (Windows/Linux)  
- ✅ Azure Recovery Services Vault  
- ✅ Azure Backup Policy  
- ✅ Azure Storage Account (ZRS)  
- ✅ Cross-Region Restore (CRR)

---

## 🌍 Regions Used  

- **Primary Region:** East US  
- **Secondary (Recovery) Region:** West US

---

## 🛠️ Key Steps Performed  

1. Created **Recovery Services Vault** in East US  
2. Enabled **Cross-Region Restore (CRR)**  
3. Configured **Backup for VM** using a custom backup policy  
4. Performed **On-Demand Backup** to generate recovery point  
5. Created **ZRS Storage Account** in West US (for restore staging)  
6. Restored VM to **Secondary Region** with a new name: `CRR-VM-DR`  
7. Tested **VM Connectivity** using Public IP + Username/Password  
8. Disabled **Soft Delete** to clean up restore points  
9. Deleted all test resources post validation

---

## 🧭 Architecture / Cross-Region Restore Flow

