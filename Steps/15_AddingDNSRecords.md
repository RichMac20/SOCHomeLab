# Create A and MX Records (DC1): <img width="284" height="178" align="right" alt="download" src="https://github.com/user-attachments/assets/9d1b0635-c2f5-4bf1-96df-72ff3cdb9a2e" />
- Add DNS A/MX Records in DNS Manager
  - On DC1
    - DNS Manager
    - Right Click homelab.local 
    - Add A record, Name=mail, IP address=DC1 (192.168.50.101) 
    - Check ‘Create associated PTR record’ 
    - Used for reverse DNS lookup, acts as anti-spam mechanism 
    - Add MX Record 
    - Right click homelab.local 
    - Select MX Record 
    - Leave “Host or child domain blank” 
    - Set FQDN to mail.homelab.local or use browse to select A record for mail, leave priority default (10). 
# Verify MX Record via NSLookup: 
- Nslookup via CMD 
- Enter “set type=MX” 
- Enter “homelab.local”
  - Should show mail exchanger and IP, which verifies records works. 
