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
  - SMTP From (What recipient sees): john@mc.com
  - Host: 127.0.0.1 
  - Click Send Test Email 
  - Provide Bill@mail.homelab.local 
    - Confirm Bill’s mailbox received the email
