# hamk_linux_management
hamk_linux_management
## Assingment 1
### Azure Virtual Machine Setup
#### I added my HAMK student email to my personal GitHub account by following these two steps:
-I accessed the Settings
-I added the email under the Emails section.

### Azure Account Setup
- Created Azure account using HAMK student email at portal.azure.com
- Activated Azure for Students subscription for additional credits

### Virtual Machine Creation
- Image: Ubuntu Server 24.04 LTS gen 2 (Canonical)
- Name: Ubuntu1-tja-NEur-B1s
- Size: Standard_B2ls_v2
- Authentication: SSH key
- Network: New resource group and subnet created
- Security: Configured to allow SSH traffic from specified IP

![vmachine overview](images/ass1_virtual_m_overview.png)

### SSH Connection Setup with PuTTY
Converting .PEM to .PPK
- Launched PuTTYgen from Start menu
- Selected RSA as the key type
- Clicked 'Load' and changed file filter to 'All Files'
- Located and selected the .pem file from Azure
- Clicked 'Save private key'
- Confirmed saving without passphrase
- Saved the converted key with .ppk extension

![PuTTY Connection](images/Ass1_putty_connection.jpg)

### Establishing SSH Connection
- Opened PuTTY
- Entered VM's public IP address in the Host Name field
- Navigated to Connection > SSH > Auth
- Browsed and selected the converted .ppk key file
- Clicked 'Open' to start the session
- Successfully connected to the VM using the specified username

Connection Verification
- Successfully logged into the Ubuntu VM shell
- Verified system access and basic functionality
- System settings left at default as per instructions

Notes
- VM created according to Microsoft Azure course specifications
- All security best practices followed
- SSH key authentication used for enhanced security