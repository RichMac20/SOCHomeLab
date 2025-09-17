# Virtualbox Setup <img width="50" height="100" alt="download" src="https://github.com/user-attachments/assets/10b1befd-9424-46ff-b10b-00524ad4780d" />
### Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads) 
### Download:
  - [Windows Server 2022](https://www.microsoft.com/en-us/evalcenter/download-windows-server-2022)
  - [Windows 10](https://www.microsoft.com/en-us/software-download/windows10) Windows forces the use of Installation Media tool, just follow the steps to get the ISO file
  - [Kali Linux](https://www.kali.org/get-kali/#kali-virtual-machines) Select download for Virtualbox
  - [pfSense](https://www.pfsense.org/download/) Forces download now through Netgate Installer, follow steps to get ISO file
  - [Security Onion](https://github.com/Security-Onion-Solutions/securityonion/blob/master/VERIFY_ISO.md) Install the ISO Image
  - [Ubuntu (Splunk)](https://ubuntu.com/download/desktop) Download latest Ubuntu Desktop version
### Create 6 VMs, one for each of the above ISO files 
VM Settings for Each:
  - Allocate 3GB of RAM per VM 
    - 12GB for SecurityOnion 
    - 4GB for Splunk
  - Allocate 2 Processors per VM
  - Allocate 30GB of Storage per VM for Windows Server/Windows 10/Kali Linux
    - Automatically set to ‘dynamically allocated’ to change based on needs
  - Allocate 10GB of Storage for pfSense
    - Automatically set to ‘dynamically allocated’ to change based on needs
  - Allocate 100GB of Storage for Security Onion
    - Automatically set to ‘dynamically allocated’ to change based on needs
  - Allocate 50GB of Storage for Splunk
    - Automatically set to ‘dynamically allocated’ to change based on needs
### Change Boot Order:
  - Change boot order to Hard disk first then ISO
    - Hardisk first, then ISO. Uncheck everything else
