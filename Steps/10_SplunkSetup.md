# Splunk Setup  <img width="100" height="75" alt="download" src="https://github.com/user-attachments/assets/de3f50a2-4bdc-4739-b99c-946b1ddc4fc9" /> 
- Install Free Splunk Enterprise from [Splunk Enterprise](https://www.splunk.com/en_us/download/splunk-enterprise.html)
  - Install as a tgz
- Open Terminal and navigate to Downloads directory
  - ‘Cd Downloads/’
- Extract the contents of the file
  - ‘Tar xvzf  (filename)’
- Change to Splunk Directory
  - ‘Cd splunk’
- Change to Splunk Bin directory
  ‘Cd bin’ 
- Start Splunk Instance
  - ‘./splunk start’
- Use a spacebar to move through the General Terms. 
- Accept terms
- Create Admin account
- Access Splunk Console via http://splunk:8000
- While in the /Downloads/splunk/bin directory, perform the following command:
  - ‘Sudo ./splunk enable boot-start’
    - Allows splunk to run on boot to prevent having to manually start splunk
