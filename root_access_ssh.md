### To enable SSH access for the root user on  Ubuntu server,
>sudo -i

>passwd
*set your password for root user*

>nano /etc/ssh/sshd_config

>add into the file => PermitRootLogin yes

>systemctl restart sshd

>service ssh restart

>ssh root@your-server-ip
