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

### 🏗️ Project Architecture

![Architecture Diagram](https://github.com/Ramya-S-M/Azure-Projects/blob/f0e73d55ab0a2a5d7442aee640e48b387fa5b640/Cross-Region%20Backup%20%26%20Restore/Architecture.png)

---

### 🛠️ Step 1: Azure VM (Source Region)

![Step 1 - VM Creation](https://github.com/Ramya-S-M/Azure-Projects/blob/f0e73d55ab0a2a5d7442aee640e48b387fa5b640/Cross-Region%20Backup%20%26%20Restore/crr-step1-VM.png)

---

### 🛠️ Step 2: Recovery Services Vault (RSV)

![Step 2 - RSV Creation](https://github.com/Ramya-S-M/Azure-Projects/blob/f0e73d55ab0a2a5d7442aee640e48b387fa5b640/Cross-Region%20Backup%20%26%20Restore/crr-step2-RSV.png)

---

### 🛠️ Step 3: Virtual Network (VNet Setup in Secondary Region)

![Step 3 - VNet Setup](https://github.com/Ramya-S-M/Azure-Projects/blob/f0e73d55ab0a2a5d7442aee640e48b387fa5b640/Cross-Region%20Backup%20%26%20Restore/crr-step3-VNET.png)

---

### 🛠️ Step 4: Storage Account (ZRS) for Restore

![Step 4 - Storage Account](https://github.com/Ramya-S-M/Azure-Projects/blob/f0e73d55ab0a2a5d7442aee640e48b387fa5b640/Cross-Region%20Backup%20%26%20Restore/crr-step4-SA.png)

---

### 🛠️ Step 5: Restore VM to Secondary Region

![Step 5 - Restore VM](https://github.com/Ramya-S-M/Azure-Projects/blob/f0e73d55ab0a2a5d7442aee640e48b387fa5b640/Cross-Region%20Backup%20%26%20Restore/crr-step5-Restore%20VM.png)

---

### ✅ Step 6: Restored VM Output (Validation)

![Step 6 - Output Screenshot](https://github.com/Ramya-S-M/Azure-Projects/blob/f0e73d55ab0a2a5d7442aee640e48b387fa5b640/Cross-Region%20Backup%20%26%20Restore/crr-step6-Output.png)

