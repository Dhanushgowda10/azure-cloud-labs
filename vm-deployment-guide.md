# Azure Virtual Machine Deployment Guide

## Objective

The objective of this guide is to provide a clear, step-by-step approach to deploying Virtual Machines (VMs) efficiently and securely in Azure. It aims to equip IT professionals, system administrators, and DevOps engineers with the necessary knowledge and best practices to plan, configure, deploy, and manage VMs.

This guide ensures consistency, scalability, and optimal performance in VM deployments, while aligning with organizational IT policies and cloud architecture standards.

---

## Task 1: Deployment of VM

In this exercise, you will be deploying a Virtual Machine.

### Step 1: Navigate to Virtual Machines

1. On the Azure portal, click on the search bar
2. Search for **Virtual machine**
3. Select **Virtual machine** from the results

### Step 2: Create a New Virtual Machine

1. In the Compute infrastructure Virtual machines tab, click on **Create** dropdown button
2. Select **Azure Virtual machine**

### Step 3: Fill in the Basic Tab

In the Basic tab, fill in the following details:

| Setting | Value |
|---------|-------|
| Subscription | Select default Subscription |
| Resource group | Select Labvm-RG |
| Virtual machine name | Enter the VM name as `lab-vm1` |
| Region | Select **West US** |
| Availability Options | Select **No infrastructure redundancy required** |
| Image | Select **Windows Server** (x64) |
| Size | Select **Standard-D2s-v3** - 2 vcpus, 8 GiB memory |
| Username | Provide username as `azureadmin` |
| Password | Create a strong password and confirm it |
| Public inbound ports | Select **Allow selected ports** |
| Select inbound ports | Select **RDP (3389)** from the dropdown |
| Licensing | Check both the license boxes |

Click **Next: Disk** to continue.

### Step 4: Configure Disks

1. In the Disks tab, select **Standard SSD (locally-redundant storage)** as the OS Disk type
2. Click **Next: Networking**

### Step 5: Configure Networking

1. Review the newly created Virtual Network and Subnet (created by default)
2. Click **Review + Create**

### Step 6: Create the Virtual Machine

1. After the validation passes, click **Create**
2. Wait for the deployment to complete

### Step 7: Access the Virtual Machine

1. Once deployment is complete, click **Go to resource**
2. Click on the dropdown beside **Connect** and select **Connect**
3. Click **Download RDP file**
4. Open the downloaded RDP file
5. Click **Connect**
6. Enter your password (the one you created during VM setup)
7. Click **Yes** to accept the certificate warning

---

## Summary

Congratulations! The virtual machine has been successfully created and initialized. You have now transitioned into its environment and are currently operating within the confines of your newly provisioned virtual machine instance.

### Key Takeaways:
- Created a Windows Server VM in Azure
- Configured networking and security settings
- Established RDP connection to the VM
- Learned best practices for VM deployment
