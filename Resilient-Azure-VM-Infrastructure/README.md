# Deploying and Managing a Resilient Azure VM Infrastructure

This project demonstrates how to design and deploy a **resilient, secure, and highly available Azure Virtual Machine (VM) infrastructure** using various Azure services and best practices.

---

## Objectives

- Deploy Azure VMs in **multiple Availability Zones**
- Ensure **load balancing** and high availability using Azure Load Balancer
- Configure **Just-in-Time (JIT)** VM Access for secure access
- Implement **monitoring and alerting** for proactive issue detection
- Apply **role-based access control (RBAC)** and NSG for security

---

## Architecture Overview

![Architecture](https://github.com/Ramya-S-M/Azure-Projects/blob/17b3d4c8343216f06af4017c4c4f274d7fb4b8a6/Resilient-Azure-VM-Infrastructure/images/architecture.png)

---

## Step-by-Step Implementation

### 1. Resource Group and Virtual Network
- Created a **Resource Group** for all components
- Created a **Virtual Network (VNet)** with subnets

### 2. Deploy Azure VMs
- Deployed **two VMs** in separate Availability Zones (Zone 1 and Zone 2)
- Installed a simple web server (IIS/Nginx)

### 3. Configure Azure Load Balancer
- Created a **Public Load Balancer**
- Added a **Backend Pool** with both VMs
- Created a **Load Balancing Rule** on port 80 (HTTP)

### 4. Enable Secure Access
- Enabled **JIT VM Access** via Microsoft Defender for Cloud
- Applied **Network Security Group (NSG)** rules for restricted access
- Configured **RBAC** to allow limited access to specific users

### 5. Enable Monitoring and Alerts
- Enabled **Azure Monitor** and connected VM diagnostics to **Log Analytics Workspace**
- Created **Alerts** for CPU utilization and VM availability
- Configured **Action Groups** to receive email/SMS alerts

---

## 📸 Screenshots

![Availability Set](https://github.com/Ramya-S-M/Azure-Projects/blob/17b3d4c8343216f06af4017c4c4f274d7fb4b8a6/Resilient-Azure-VM-Infrastructure/images/Availability-Set.png)

![Load Balancer](https://github.com/Ramya-S-M/Azure-Projects/blob/17b3d4c8343216f06af4017c4c4f274d7fb4b8a6/Resilient-Azure-VM-Infrastructure/images/Load-Balancer.png)

![Virtual Machine](https://github.com/Ramya-S-M/Azure-Projects/blob/17b3d4c8343216f06af4017c4c4f274d7fb4b8a6/Resilient-Azure-VM-Infrastructure/images/Virtual-Machine.png)

![Monitor-Action Group](https://github.com/Ramya-S-M/Azure-Projects/blob/17b3d4c8343216f06af4017c4c4f274d7fb4b8a6/Resilient-Azure-VM-Infrastructure/images/actiongroup.png)

![Load Balancer Output](https://github.com/Ramya-S-M/Azure-Projects/blob/17b3d4c8343216f06af4017c4c4f274d7fb4b8a6/Resilient-Azure-VM-Infrastructure/images/load-balancer-output.png)

![SSH Output](https://github.com/Ramya-S-M/Azure-Projects/blob/17b3d4c8343216f06af4017c4c4f274d7fb4b8a6/Resilient-Azure-VM-Infrastructure/images/ssh-output.png)

![Virtual Network](https://github.com/Ramya-S-M/Azure-Projects/blob/17b3d4c8343216f06af4017c4c4f274d7fb4b8a6/Resilient-Azure-VM-Infrastructure/images/vnet.png)
