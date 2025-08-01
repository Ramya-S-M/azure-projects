# 🖥️ Deploy Azure VM Using Shared Image Gallery (SIG)

This project demonstrates how to create a reusable VM image and distribute it across regions using **Azure Shared Image Gallery (SIG)**.

It helps in deploying consistent VM configurations at scale, useful in enterprise environments and Dev/Test setups.

---

# azure-projects

This repo contains my self-learned Azure projects covering VMs, Storage, Backup, Networking, Monitoring, and Security.

---

## 📌 Project 1: Deploy Azure VM with Shared Image Gallery

## Step 1: Base VM Created
![Base VM Created]("\azure-vm-shared-image-gallery\project-01-vm-shared-image-gallery\images\Base_VM_Created.png.png")

## Step 2: Connected to VM and Deprovisioned
![Connected to VM and Deprovisioned]("\azure-vm-shared-image-gallery\project-01-vm-shared-image-gallery\images\Connected_to_VM_and_Deprovisioned.png.png")

## Step 3: Shared Image Gallery Created
![Shared Image Gallery Created]("\azure-vm-shared-image-gallery\project-01-vm-shared-image-gallery\images\Shared_Image_Gallery_Created.png.png")

## Step 4: Image Version Created in SIG
![Image Version Created in SIG]("\azure-vm-shared-image-gallery\project-01-vm-shared-image-gallery\images\Image_Version_Created_in_SIG.png.png")

## Step 5: New VM Deployed from SIG
![New VM Deployed from SIG]("\azure-vm-shared-image-gallery\project-01-vm-shared-image-gallery\images\New_VM_Deployed_from_SIG.png.png")

## Step 6: Verified New VM Working
![Verified New VM Working]("\azure-vm-shared-image-gallery\project-01-vm-shared-image-gallery\images\Verified_New_VM_Working.png.png")


---

## 🚀 Azure Services Used

- Azure Virtual Machines  
- Shared Image Gallery  
- Resource Groups  
- Azure Compute Gallery  
- Azure Disk Images

---

## 🪜 Step-by-Step Execution

### 1. Create Base VM
- Region: East US (or your preferred region)  
- OS: Ubuntu LTS  
- Authentication: SSH Public Key  

### 2. Optional Configuration
- SSH into VM  
- Run setup/config commands (optional)  

### 3. Deprovision the VM

```bash
sudo waagent -deprovision+user --force  
sudo shutdown -h now
