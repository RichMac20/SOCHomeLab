# Allow SMTP(25)/IMAP(143) to DC1’s Incoming/Outgoing Firewall Rules (DC1):  
- Firewall <img width="200" height="200" align="right" alt="download" src="https://github.com/user-attachments/assets/e7c6144b-22b4-4385-8da3-6fd09335eb6d" />
  - Rules 
  - Add 
  - Specify SMTP/port 25 
  - Add 
  - Specify IMAP/port 143. 
- Test new firewall rules using the Powershell command 
  - ‘Test-NetConnection -ComputerName 192.168.50.101 [25/143]’ 
    - If Status comes back as “True” then it works. 
