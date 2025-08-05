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

![Availability Set](https://github.com/Ramya-S-M/Azure-Projects/blob/669caad688d67e3966d804021b3125c72aa96c6c/Resilient%20Azure%20VM%20Infrastructure/Availability%20Set.png)

![Load Balancer](https://github.com/Ramya-S-M/Azure-Projects/blob/669caad688d67e3966d804021b3125c72aa96c6c/Resilient%20Azure%20VM%20Infrastructure/Load%20Balancer.png)

![Virtual Machine](https://github.com/Ramya-S-M/Azure-Projects/blob/669caad688d67e3966d804021b3125c72aa96c6c/Resilient%20Azure%20VM%20Infrastructure/Virtual%20Machine.png)

![Monitor-Action Group](https://github.com/Ramya-S-M/Azure-Projects/blob/669caad688d67e3966d804021b3125c72aa96c6c/Resilient%20Azure%20VM%20Infrastructure/actiongroup.png)

![Architecture](https://github.com/Ramya-S-M/Azure-Projects/blob/669caad688d67e3966d804021b3125c72aa96c6c/Resilient%20Azure%20VM%20Infrastructure/architecture.png)

![Load Balancer Output](https://github.com/Ramya-S-M/Azure-Projects/blob/669caad688d67e3966d804021b3125c72aa96c6c/Resilient%20Azure%20VM%20Infrastructure/load%20balancer-output.png)

![SSH Output](https://github.com/Ramya-S-M/Azure-Projects/blob/669caad688d67e3966d804021b3125c72aa96c6c/Resilient%20Azure%20VM%20Infrastructure/ssh-output.png)

![Virtual Network](https://github.com/Ramya-S-M/Azure-Projects/blob/669caad688d67e3966d804021b3125c72aa96c6c/Resilient%20Azure%20VM%20Infrastructure/vnet.png)
