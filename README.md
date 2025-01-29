# Home lab
This document outlines the steps I took to create a home lab environment for practicing cybersecurity skills. The lab consists of a Windows 10 laptop running Oracle VirtualBox with Ubuntu as the primary virtual machine (VM). This setup allows me to simulate real-world scenarios, test tools, and practice vulnerability management, penetration testing, and incident response.

<div align="center">
  <img src="https://github.com/30Gramz/Home-lab/blob/374b2f5381915422eebdb2424fee292987ae71b3/Homelab.drawio.png" alt="Home Lab Set-up" width="500">
</div>



# Steps 

# Step 1: Setting Up the Host Machine
Hardware Specifications:

- Laptop: Windows 10 (64-bit)

- Processor: Intel Core i5 (or equivalent)

- RAM: 8GB (minimum recommended for running VMs)

- Storage: 256GB SSD (for faster performance)

- Install Oracle VirtualBox:

- Downloaded Oracle VirtualBox from the <a href="https://www.virtualbox.org/"> Virtualbox official website</a>.

- Installed VirtualBox on the Windows 10 laptop, ensuring all default settings were selected.

- Verified the installation by launching VirtualBox and checking for any errors.

 # Step 2: Downloading and Installing Ubuntu
Download Ubuntu ISO:

Downloaded the latest Ubuntu Server ISO from the <a href="https://ubuntu.com/download/desktop"> Official Ubuntu website </a>  

Chose the LTS (Long-Term Support) version for stability.

Create a New Virtual Machine:

Opened VirtualBox and clicked New to create a new VM.

Named the VM Ubuntu-Server and selected Linux as the type and Ubuntu (64-bit) as the version.

Allocated 2GB of RAM and created a 20GB virtual hard disk (VDI format, dynamically allocated).

Install Ubuntu on the VM:

Attached the Ubuntu ISO to the VM by going to Settings > Storage > Optical Drive and selecting the downloaded ISO.

Started the VM and followed the Ubuntu installation prompts:

Selected Install Ubuntu.

Configured the network settings (used DHCP for simplicity).

Partitioned the disk using the default settings.

Set up a user account with a strong password.

Completed the installation and rebooted the VM.
