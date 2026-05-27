1.Groups:A group is used to give permissions/access to multiple users together.

To view existing groups
```bash
cat /etc/group
```
Create a group
```bash
groupadd ece
```
Create user
```bash
adduser student1
```
Add user to group
```bash
usermod -aG ece student1
```
2.SSH:SSH(Secure shell) is used to securely connect/login to remote linux servers.

Check SSH client
```bash
SSH
```
Check SSH service status
```bash
systemctl status ssh
```
Verify SSH configuration file
```bash
cat /etc/ssh/sshd_config
```
Password authentication
```bash
grep PasswordAuthentication /etc/ssh/sshd_config
```
Root login
```bash
grep PermitRootLogin /etc/ssh/sshd_config
```
