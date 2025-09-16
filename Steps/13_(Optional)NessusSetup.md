# Installing a Vulnerability Scanner (Nessus): <img width="500" height="85" alt="download" src="https://github.com/user-attachments/assets/9aff4360-5384-4ba5-868f-62e4272eff67" />

- On Splunk (Ubunu Server):
  - Go to Tenables Nessus download page and install for the specific distribution/architecture in use 
  - Run the Curl command shown for Linux
  - Unpack via dpkg -i (filename) 
  - -i Installs the file
  - Start the service: “systemctl start nessusd”
  - Enable to run on boot “systemctl enable nessusd”
# Nessus Configuration:
- Access Nessus via https://192.168.150.20:8834
- Register with Nessus Essentials 
- Register via email 
- Create Admin Account
- Download Plugins
  - May 5 - 10 Mins
- Eventually a “Welcome to Nessus” window will appear prompts for targets
  - Enter 192.168.50.0/24 to discover all potential targets within the victim subnet 
    - Select DC1/PC1 
- Nessus will then run a Basic Network Scan 
