# Lab Environment Setup

## Objective
To build a safe, isolated, and scalable virtual environment for performing penetration testing and ethical hacking exercises.

## Theory & Concepts
- **Virtualization**: Using software to create an abstracted layer over computer hardware, allowing for the creation of Virtual Machines (VMs).
- **Hypervisors**: Software that creates and runs virtual machines (e.g., VirtualBox, VMware).
- **Network Modes**:
  - **NAT**: Shared internet access through the host.
  - **Host-Only**: Isolated network between host and virtual machines (recommended for security labs).
  - **Bridged**: VM appears as a physical device on the local network.

## Tools Used
- Oracle VM VirtualBox
- Kali Linux (Attacker Machine)
- Metasploitable2 (Target Machine)

## Commands & Practical Steps
1. **Host-Only Network Creation**:
   - Open VirtualBox → File → Host Network Manager → Create.
   - Assign IP range: `192.168.56.0/24`.
2. **VM Import**:
   - Download Kali Linux `.ova` and Metasploitable2 `.zip`.
   - File → Import Appliance (for Kali).
3. **Network Configuration**:
   - Settings for both VMs → Network → Adapter 1 → Host-Only Adapter.
4. **Verifying Connectivity**:
   ```bash
   # On Kali
   ip addr show
   ping 192.168.56.101 # (Check Metasploitable IP)
   ```

## Practical Demonstration Summary
Successfully installed and configured the virtualization environment. Verified that the attacker machine (Kali) can communicate with the target machine (Metasploitable2) over a private, isolated network.
