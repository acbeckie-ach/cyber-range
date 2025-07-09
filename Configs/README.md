# VM Configuration Files (`.vmx`)

This folder contains `.vmx` configuration files for the virtual machines used in the cyber range project. These files define VM properties such as memory, CPU, guest OS type, and network settings.

## List of VMs

| File Name     | Description                            |
|---------------|----------------------------------------|
| `lab_01.vmx`  | Infection Monkey simulation VM         |
| `lab_02.vmx`  | DVWA + ZAP in Docker container         |
| `lab_03.vmx`  | WordPress + Nikto scanning             |
| `lab_04.vmx`  | WebGoat + Contrast Security            |
| `lab_05.vmx`  | Nessus scanning node                   |
| `gns3_lab.vmx`| GNS3 VM for emulated network topology  |
| `ansible_control_node` |Manages deployment and 
 ochestration of all cyber range scenarios 		 |

> The `.vmx` files do not include virtual disk files (`.vmdk`). 

- `lab_01.vmx` – Ubuntu 18.04 VM simulating a breach scenario using Infection Monkey to test lateral movement and vulnerability mapping.
- `lab_02.vmx` – Ubuntu 18.04 VM running Docker containers for DVWA and OWASP ZAP, used for dynamic web application testing.
- `lab_03.vmx` – Ubuntu 18.04 VM running WordPress on Apache, targeted by Nikto for vulnerability scanning.
- `lab_04.vmx` – Ubuntu 18.04 VM configured with WebGoat and Contrast Security for application vulnerability and behavior analysis.
- `gns3_lab.vmx` – GNS3 network virtualization appliance (Ubuntu 20.04), used for emulating segmented red/blue/cloud network zones.

- `control_terminal.vmx` – Ubuntu 20.04 VM used as the Ansible control node. Manages deployment of all cyber range scenarios.





