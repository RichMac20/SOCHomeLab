# Add Users to Domain (DC1) <img width="50" height="50" alt="download" src="https://github.com/user-attachments/assets/79726ec2-4d77-4c8b-abca-60190640e3c6" /> 
- Click homelab.local Dropdown Menu
- Select Users
- Right-Click and Select New User 
- Add ‘Bill’ and ‘Fred’ to the homelab.local Domain
  - Used ‘Bill’ and ‘Fred’ as Logon to keep it simple 
# Setup Windows 10 Pro (PC1): 
- In Virtualbox Manager
  - Change Network Adapter 2 to Internal Network for LAN1
- Boot/Setup Windows 10
  - Select Windows 10 Pro 
  - Allow Default Storage Allocation 
  - Setup Offline Admin Account 
- Rename PC via About Your PC to PC1 
- Reboot
- Install Virtualbox Guest Additions 
  - Enhances performance/usability 
- Change IPV4 Ethernet Adapter to use DC1s IP (192.168.50.101) as primary DNS server
  - Will still use pfSense as a backup if it can’t resolve locally
# Join PC1 to homelab.local Domain: 
### Note: Step is only necessary if PC1 didn’t automatically join domain through previous pfSense configuration
- Open ‘About Your PC’ 
- Select Advanced System Settings
- Select Change 
  - Select Domain and enter homelab.local
  - Enter Admin Credentials 
- Reboot PC1
