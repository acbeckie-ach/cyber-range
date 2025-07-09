# Deployment Guide for Cyber Range Using Ansible and VMware

This guide outlines how to deploy the automated cyber range lab environment, as described in the paper:  
**"Security Scenarios Automation and Deployment in Virtual Environment using Ansible" (DOI: [10.1109/COMM54429.2022.9817150](https://doi.org/10.1109/COMM54429.2022.9817150))**

---

## Prerequisites

- **Host Environment**:  
  - VMware Workstation Pro (16+)
  - External drive with >150GB free space (for 7+ VMs)
  - Ubuntu-based Ansible Control VM (preconfigured)

- **VM Infrastructure**:  
  - VMware ESXi Server running inside Workstation
  - Pre-deployed VMs (lab_01 to lab_06, GNS3_VM, Control_Terminal_1)
  - Properly configured .vmx and .vmdk files (see `configs/`)

- **Network Configuration**:  
  - vSwitch with VLAN segmentation: `gns3`, `VM Network`, `Management`
  - Static IP assigned to ESXi (e.g., `192.168.72.128`)
  - GNS3 Web UI accessible via host browser

---

## Project Structure

project-root/
├── ansible/
│ ├── inventory.yml
│ ├── playbooks/
│ │ ├── deploy.yml
│ │ └── configure_services.yml
├── configs/
│ ├── lab_01.vmx
│ ├── lab_02.vmx
│ └── ...
├── diagrams/
│ ├── architecture-overview.png
│ ├── gns3-topology.png
│ └── ansible-flowchart.svg
├── docs/
│ ├── deployment.md
│ └── usage.md
└── README.md

## Step 1: Configure Inventory
located at: `ansible/inventory.yml

## Step 2: Create VMs Using Ansible
located at: `ansible/playbooks/deploy-vm.yml

## Step 3: Run Security Scans
located at: `zap_scan.yml`