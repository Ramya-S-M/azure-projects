# 🚀 Deploying and Managing a Resilient Azure VM Infrastructure

This project demonstrates how to design and deploy a **resilient, secure, and highly available Azure Virtual Machine (VM) infrastructure** using various Azure services and best practices.

---

## 🎯 Objectives

- Deploy Azure VMs in **multiple Availability Zones**
- Ensure **load balancing** and high availability using Azure Load Balancer
- Configure **Just-in-Time (JIT)** VM Access for secure access
- Implement **monitoring and alerting** for proactive issue detection
- Apply **role-based access control (RBAC)** and NSG for security

---

## 🏗️ Architecture Overview



---

## 🔧 Step-by-Step Implementation

### 1️⃣ Resource Group and Virtual Network
- Created a **Resource Group** for all components
- Created a **Virtual Network (VNet)** with subnets

### 2️⃣ Deploy Azure VMs
- Deployed **two VMs** in separate Availability Zones (Zone 1 and Zone 2)
- Installed a simple web server (IIS/Nginx)

### 3️⃣ Configure Azure Load Balancer
- Created a **Public Load Balancer**
- Added a **Backend Pool** with both VMs
- Created a **Load Balancing Rule** on port 80 (HTTP)

### 4️⃣ Enable Secure Access
- Enabled **JIT VM Access** via Microsoft Defender for Cloud
- Applied **Network Security Group (NSG)** rules for restricted access
- Configured **RBAC** to allow limited access to specific users

### 5️⃣ Enable Monitoring and Alerts
- Enabled **Azure Monitor** and connected VM diagnostics to **Log Analytics Workspace**
- Created **Alerts** for CPU utilization and VM availability
- Configured **Action Groups** to receive email/SMS alerts

---

## 📸 Screenshots

> Include the following screenshots (optional):
- VM deployment in Availability Zones
- Load Balancer backend pool
- JIT Access enabled
- Alert rule creation
- Metrics in Azure Monitor
