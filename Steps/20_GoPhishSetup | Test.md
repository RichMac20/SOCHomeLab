# Setup GoPhish:  <img width="200" height="200" align="right" alt="download" src="https://github.com/user-attachments/assets/70813151-dba8-4566-84de-1d1a630db868" />
- Launch terminal
- Enter ‘gophish’ 
  - Should launch a webpage
- Login with default creds provided via the terminal (Password may vary based on version)
- Set new Password
# Setup Sending Profiles for Test Email via GoPhish (Kali):
- Select “Sending Profiles” 
- Select New Profile 
  - Enter Postfix Test
  - SMTP From (What recipient sees): john@mail.mc.com
  - Host: 172.16.0.10:25 
  - Click Send Test Email 
  - Provide Bill@mail.homelab.local 
    - Confirm Bill’s mailbox received the email
  - Note: If there are issues with sending a test email, check the [Config](https://github.com/RichMac20/SOCHomeLab/blob/main/Steps/Configs/main.cf) file for Postfix in /etc/postfix/main.cf
