
### create new user with sudo privileges 

```bash 
sudo adduser username
```
Grant privilages.
```bash
sudo usermod -aG sudo username
```
Use the su command to switch to the new user account.

```bash
su - username
```
#### Usefull ssh commands

Use this command to remove entries from known_hosts:
```bash
ssh-keygen -R hostname
# works with ips as well
```

Create file authorized_keys and copy data to it from the root file. It can be done via 

```bash
rsync --archive --chown=sammy:sammy ~/.ssh /home/sammy
```

https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-18-04

https://www.digitalocean.com/community/tutorials/automating-initial-server-setup-with-ubuntu-18-04
