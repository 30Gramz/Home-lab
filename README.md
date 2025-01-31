<div align="center">
<img src="https://github.com/30Gramz/Home-lab/blob/265186f0b3f4d2c469402b65ddd8b7760030015d/hq720.jpg">
</div>

# Home lab
This document outlines the steps I took to create a home lab environment for practicing cybersecurity skills. The lab consists of a Windows 10 laptop running Oracle VirtualBox with Ubuntu as the primary virtual machine (VM). This setup allows me to simulate real-world scenarios, test tools, and practice vulnerability management, penetration testing, and incident response.

## Visualization
<div align="center">
  <img src="https://github.com/30Gramz/Home-lab/blob/53a44fe1a1babd63f9d5917f346cc5eb6fabe390/Untitled%20Diagram.drawio.png" alt="Home Lab Set-up" width="400">
</div>



# Steps 

## Step 1: Setting Up the Host Machine
*Hardware Specifications:*

- Laptop: Windows 10 (64-bit)

- Processor: Intel Core i5 (or equivalent)

- RAM: 8GB (minimum recommended for running VMs)

- Storage: 256GB SSD (for faster performance)

### Install Oracle VirtualBox:

- Downloaded Oracle VirtualBox from the <a href="https://www.virtualbox.org/"> Virtualbox official website</a>.

- Installed VirtualBox on the Windows 10 laptop, ensuring all default settings were selected.

- Verified the installation by launching VirtualBox and checking for any errors.

 ## Step 2: Downloading and Installing Ubuntu
### Download Ubuntu ISO:

- Downloaded the latest Ubuntu Server ISO from the <a href="https://ubuntu.com/download/desktop"> Official Ubuntu website </a>  

- Chose the LTS (Long-Term Support) version for stability.

### Create a New Virtual Machine:

- Opened VirtualBox and clicked New to create a new VM.

- Named the VM Ubuntu-Server and selected Linux as the type and Ubuntu (64-bit) as the version.

- Allocated 2GB of RAM and created a 20GB virtual hard disk (VDI format, dynamically allocated).

### Install Ubuntu on the VM:

- Attached the Ubuntu ISO to the VM by going to Settings > Storage > Optical Drive and selecting the downloaded ISO.

- Started the VM and followed the Ubuntu installation prompts:

Selected Install Ubuntu.

Configured the network settings (used DHCP for simplicity).

Partitioned the disk using the default settings.

Set up a user account with a strong password.

- Completed the installation and rebooted the VM.

## Post-Installation Setup:

Updated the system using the command:

 <img src="https://github.com/30Gramz/Home-lab/blob/eb8fad22ea56265f2e49ab39166a7c4c3c322e8e/update%20command.png">

Installed essential tools like curl, git, and vim:

 <img src="https://github.com/30Gramz/Home-lab/blob/6f4bb4c25111574333516409031ac5627a2d307e/update%20command%202.png">

 ## Step 3: Configuring the Ubuntu VM for Security Testing

### Install OpenSSH Server:

- Installed OpenSSH to enable remote access:

  <img src="https://github.com/30Gramz/Home-lab/blob/70abc365c8595d4c8622f3ad4edca3729de8140e/Annotation%202025-01-31%20095127.png">
  
- Enabled and started the SSH service:

  <img src="https://github.com/30Gramz/Home-lab/blob/ac5ef5686a9a60fb02d293e322df27e316785d54/Annotation%202.png">

- Verified the SSH service is running:

  <img src="https://github.com/30Gramz/Home-lab/blob/893bdd2894b72adf33b6a1c7ddfdedf42e47adae/Annotation%203.png">


### Configure Firewall (UFW):

- Installed and enabled UFW (Uncomplicated Firewall):

  <img src="https://github.com/30Gramz/Home-lab/blob/5855fa6695ca740947568e23f4733e18776f0203/Annotation%204.png">

- Allowed SSH through the firewall:

  <img src="https://github.com/30Gramz/Home-lab/blob/7ce8f39c6848ee04650ff63dd712d42265d839dd/Annotation%205.png">

- Checked the status of UFW:

  <img src="https://github.com/30Gramz/Home-lab/blob/863e3d9f2657b9f0e0b56af0bef96dcb6cbf4d37/Annotation%206.png">


### Install Security Tools:

- Installed common security tools for penetration testing:

  <img src="https://github.com/30Gramz/Home-lab/blob/38d3246c5c1b8997a136513534f73592bfec747a/Annotation%207.png">

- For Wireshark, allowed non-superusers to capture packets:
  
  <img src="https://github.com/30Gramz/Home-lab/blob/5dd28023f2cbbda1065bf52f18ce0c223b334b44/Annotation%208.png">

- Registered on the Qualys community edition

  A free version of Qualys' cloud-based security and compliance solutions, designed to help individuals, small teams, and cybersecurity enthusiasts explore and utilize Qualys' tools for vulnerability management and other security tasks. 

  

  


