# Ansile 

#### first install ansible on your control server.and after that install on your destination server

#### install ansible ubuntu

  

> sudo apt-add-repository ppa:ansible/ansible

> sudo apt update

> sudo apt install ansible

#### path of your installation

- /etc/ansible

#### Prioritize reading settings in ansible
- ANSIBLE-CONFIG(environment variable if set)
- ansible.cfg
- ~/.ansible.cfg
- /etc/ansible/ansible.cfg

#### create user for ansible in your others servers you can use root user in ansible.cfg

> sudo adduser ansible

> cd /etc/sudoers.d/

> visudo ansible

after that write this  for more privilage for ansible user in */etc/sudoers.d*

>nano ansible

>ansible ALL=(ALL:ALL) NOPASSWD:ALL

#### Set up your SSH on other servers for Control node

>ssh-keygen -t ed25519 -b 4096 -a 200 -C "your_email@example.com"

>ssh-copy-id -i ~/.ssh/id_ed25519.pub root@remote-server
