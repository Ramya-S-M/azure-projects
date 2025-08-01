# 🖥️ Deploy Azure VM Using Shared Image Gallery (SIG)

This project demonstrates how to create a reusable VM image and distribute it across regions using **Azure Shared Image Gallery (SIG)**.

It helps in deploying consistent VM configurations at scale, useful in enterprise environments and Dev/Test setups.

---

# azure-projects

This repo contains my self-learned Azure projects covering VMs, Storage, Backup, Networking, Monitoring, and Security.

---

## 📌 Project 1: Deploy Azure VM with Shared Image Gallery

This project demonstrates how to create and manage Azure Virtual Machines using a Shared Image Gallery (SIG) for standardized, scalable image distribution across regions.

1. Created a Generalized VM to capture a custom image.

2. Created an Image Definition and Image Version inside a Shared Image Gallery.

3. Deployed a new VM using that Shared Image version.

4. Ensured versioning, scalability, and regional replication for faster and consistent VM deployments.

###This setup helps in managing golden images for your organization and supports large-scale VM deployments using pre-approved configurations.

## Step 1: Base VM Created
![Base VM Created](https://github.com/Ramya-S-M/Shared-Image-Gallery-SIG-VM/blob/3f1629325e3a6342a9ea7ae5ee290cfcf983dce6/images/Base_VM_Created.png)

## Step 2: Connected to VM and Deprovisioned
![Connected to VM and Deprovisioned](https://github.com/Ramya-S-M/Shared-Image-Gallery-SIG-VM/blob/3f1629325e3a6342a9ea7ae5ee290cfcf983dce6/images/Connected_to_VM_and_Deprovisioned.png)

## Step 3: Shared Image Gallery Created
![Shared Image Gallery Created](https://github.com/Ramya-S-M/Shared-Image-Gallery-SIG-VM/blob/3f1629325e3a6342a9ea7ae5ee290cfcf983dce6/images/Shared_Image_Gallery_Created.png)

## Step 4: Image Version Created in SIG
![Image Version Created in SIG](https://github.com/Ramya-S-M/Shared-Image-Gallery-SIG-VM/blob/3f1629325e3a6342a9ea7ae5ee290cfcf983dce6/images/Image_Version_Created_in_SIG.png)

## Step 5: New VM Deployed from SIG
![New VM Deployed from SIG](https://github.com/Ramya-S-M/Shared-Image-Gallery-SIG-VM/blob/3f1629325e3a6342a9ea7ae5ee290cfcf983dce6/images/New_VM_Deployed_from_SIG.png)

## Step 6: Verified New VM Working
![Verified New VM Working](https://github.com/Ramya-S-M/Shared-Image-Gallery-SIG-VM/blob/3f1629325e3a6342a9ea7ae5ee290cfcf983dce6/images/Verified_New_VM_Working.png)


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
