# Virtualized Cyber Range for Offensive Security

This repository contains the supporting material, automation scripts, and configuration files related to the research presented in:

# Security Scenarios Automation and Deployment in Virtual Environment/Cloud using Ansible
- Rebecca Acheampong, Alexandre Rekeraho, Titus Constantin Bălan, Dorin-Mircea Popovici
- Presented at the 2022 International Conference on Communications (COMM)
- DOI: DOI: 10.1109/COMM54429.2022.9817150

# About the Project
This project automates the deployment of a virtual cyber range using Ansible, with VMs running in a nested ESXi environment inside VMware Workstation. 
It simulates red team/blue team training environments across multiple lab scenarios.

The project integrates:
- Ansible for orchestration and deployment
- Dockerized apps like DVWA, OWASP ZAP, WebGoat
- Tools like Nessus, Nikto, Infection Monkey, Contrast Security
- GNS3 for emulated network topologies

# Repository Structure
- `configs/` — `.vmx` files for each lab
- `diagrams/` — Vswitch, Ansible and sceanrio topology diagrams
- `deployment/` — Ansible playbooks for VM creation, app deployment and security tests
- `docs/` — Abstract, scenarios description

# Labs and Scenarios
- Lab Name 				Description

+ Lab_01				Infection Monkey breach simulation

+ Lab_02				OWASP ZAP scanning DVWA (Docker)

+ Lab_03				Apache + WordPress + Nikto scan

+ Lab_04				WebGoat + Contrast Security integration

+ Lab_05				Nessus vulnerability scanner

+ Lab_06				Metasploitable + Nmap reconnaissance

+ GNS3_Lab				Emulated network zones (private/public/cloud) via GNS3

- All labs were automated with Ansible playbooks and tied to MITRE ATT&CK tactics.



# Deployment instructions
- Due to size limitations, the full virtual machines (VMs) are **not included** in this repository.

- To deploy the cyber range environment:

 **Clone this repository** to get the configuration files, Ansible playbooks, and diagrams:



# License
- This project is provided for academic and research use only. For reuse or adaptation, please cite the original paper or contact the authors.
