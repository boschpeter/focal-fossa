Focal fossa

---
## 	 git clone http://admin:ThisIsCool_2020@gitlab.example.com/root/2B

````
boscp08@boscp08-HP-Compaq-8510p:~/Projects/scratch/virtual-insanity$ git clone http://admin:ThisIsCool_2020@gitlab.example.com/root/2B
Cloning into '2B'...
warning: redirecting to http://gitlab.example.com/root/2B.git/
remote: Enumerating objects: 37, done.
remote: Counting objects: 100% (37/37), done.
remote: Compressing objects: 100% (32/32), done.
remote: Total 37 (delta 5), reused 0 (delta 0), pack-reused 0
remote: 
Unpacking objects: 100% (37/37), 20.11 MiB | 1.44 MiB/s, done.
boscp08@boscp08-HP-Compaq-8510p:~/Projects/scratch/virtual-insanity$ cd 
boscp08@boscp08-HP-Compaq-8510p:~$ cat .my-credentials 
http://admin:ThisIsCool_2020@gitlab.example.com
http://admin:ThisIsCool_2020@192.168.2.11
https://ezahr:Peter%212020@github.com
https://boschpeter:Peter%212020@github.com
````

## sudo nano /etc/hosts
````
127.0.0.1       localhost
127.0.1.1       boscp08-HP-Compaq-8510p

# The following lines are desirable for IPv6 capable hosts
::1     ip6-localhost ip6-loopback
fe00::0 ip6-localnet
ff00::0 ip6-mcastprefix
ff02::1 ip6-allnodes
ff02::2 ip6-allrouters
192.168.2.14 gitlab.example.com
````

## git clone http://admin:ThisIsCool_2020@192.168.2.11/root/powerdesigner.git

````
boscp08@boscp08-HP-Compaq-8510p:~$ git clone http://admin:ThisIsCool_2020@192.168.2.11/root/powerdesigner.git
Cloning into 'powerdesigner'...
remote: Enumerating objects: 54, done.
remote: Counting objects: 100% (54/54), done.
remote: Compressing objects: 100% (51/51), done.
remote: Total 54 (delta 15), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (54/54), 28.24 MiB | 1.39 MiB/s, done.

boscp08@boscp08-HP-Compaq-8510p:~$ cat .my-credentials
http://admin:ThisIsCool_2020@192.168.2.11
https://ezahr:Peter%212020@github.com
https://boschpeter:Peter%212020@github.com
boscp08@boscp08-HP-Compaq-8510p:~$ 



````

## git clone https://ezahr:Peter\!2020@github.com/ezahr/MobileIron

````
boscp08@boscp08-HP-Compaq-8510p:~/Projects/scratch/virtual-insanity$ git clone https://ezahr:Peter\!2020@github.com/ezahr/MobileIron
Cloning into 'MobileIron'...
remote: Enumerating objects: 20, done.
remote: Counting objects: 100% (20/20), done.
remote: Compressing objects: 100% (17/17), done.
remote: Total 2405 (delta 10), reused 6 (delta 3), pack-reused 2385
Receiving objects: 100% (2405/2405), 266.63 MiB | 1.38 MiB/s, done.
Resolving deltas: 100% (1133/1133), done.
Updating files: 100% (756/756), done.
boscp08@boscp08-HP-Compaq-8510p:~/Projects/scratch/virtual-insanity$ cd 
boscp08@boscp08-HP-Compaq-8510p:~$ cat .my-credentials
https://ezahr:Peter%212020@github.com
https://boschpeter:Peter%212020@github.com
boscp08@boscp08-HP-Compaq-8510p:~$ 

````


## git clone https://boschpeter:Peter\!2020@github.com/boschpeter/focal-fossa

````
boscp08@boscp08-HP-Compaq-8510p:~$ cat .my-credentials 
https://boschpeter:Peter%212020@github.com
````

## git config --list --show-origin

| git config --list --show-origin|
|----------------------------------------------------|
|git config --global user.name "ezahr"|
|git config --global user.email "bosch.peter@icloud.com"|
|git config --global credential.helper 'store --file ~/.my-credentials'|

````
boscp08@boscp08-HP-Compaq-8510p:~$ cat .gitconfig 
[user]
	name = ezahr
	email = bosch.peter@icloud.com
[credential]
	helper = store --file ~/.my-credentials

````


## sudo apt  install tree

````
boscp08@boscp08-HP-Compaq-8510p:~/Projects$ tree
.
├── gitlab.example.com
│   └── pi8gb
└── scratch
    └── virtual-insanity

4 directories, 0 files

````

## 	sudo apt update && sudo apt install git && git --version	

[how-to-install-git-on-ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-18-04)


````
sudo apt update && sudo apt install git && git --version
````



home/boscp08/.gitconfig   user.name=boschpeter
file:/home/boscp08/.gitconfig   user.password=Peter\!2020
file:/home/boscp08/.gitconfig   user.email=bosch.peter@icloud.com
git config --global credential.helper 'store --file ~/.my-credentials'
git config --list --show-origin

---

## rsync -avz -e ssh root@192.168.2.90:/srv/www/htdocs/site/dokuwiki /var/www/html

````
crontab -l
@reboot sudo swapoff -a
*/10 * * * * rsync -avz -e ssh root@192.168.2.90:/srv/www/htdocs/site/dokuwiki /var/www/html
````

````
sent 997,163 bytes  received 1,157,098,476 bytes  1,435,952.44 bytes/sec
total size is 1,568,807,514  speedup is 1.35
boscp08@boscp08-HP-Compaq-8510p:~$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda5       466G   16G  427G   4% /
````


## crontab -e

````
boscp08@boscp08-HP-Compaq-8510p:~$ crontab -e
no crontab for boscp08 - using an empty one

Select an editor.  To change later, run 'select-editor'.
  1. /bin/nano        <---- easiest
  2. /usr/bin/vim.tiny
  3. /bin/ed

Choose 1-3 [1]: 1

````

````
# m h  dom mon dow   command
# ┌───────────── minute (0 - 59)
# │ ┌───────────── hour (0 - 23)
# │ │ ┌───────────── day of month (1 - 31)
# │ │ │ ┌───────────── month (1 - 12)
# │ │ │ │ ┌───────────── day of week (0 - 6) (Sunday to Saturday;
# │ │ │ │ │                                       7 is also Sunday on some systems)
# │ │ │ │ │
# │ │ │ │ │
# * * * * *  command to execute

````

## cat .bashrc



## 	ssh-copy-id -i ~/.ssh/id_rsa.pub root@192.168.2.90 

````
boscp08@boscp08-HP-Compaq-8510p:~/.ssh$ ssh-copy-id -i ~/.ssh/id_rsa.pub root@192.168.2.90 
/usr/bin/ssh-copy-id: INFO: Source of key(s) to be installed: "/home/boscp08/.ssh/id_rsa.pub"
The authenticity of host '192.168.2.90 (192.168.2.90)' can't be established.
ECDSA key fingerprint is SHA256:ips4bS6Q5Nl/xsd9nc+u4o2rxqXPOSWbVes1rTPwOXs.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
/usr/bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
/usr/bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
Password: 

Number of key(s) added: 1

Now try logging into the machine, with:   "ssh 'root@192.168.2.90'"
and check to make sure that only the key(s) you wanted were added.

boscp08@boscp08-HP-Compaq-8510p:~/.ssh$ ssh root@192.1698.2.90
ssh: Could not resolve hostname 192.1698.2.90: Name or service not known
boscp08@boscp08-HP-Compaq-8510p:~/.ssh$ ssh root@192.168.2.90
Last failed login: Mon Aug 24 17:42:24 CEST 2020 from 192.168.2.6 on ssh:notty
There was 1 failed login attempt since the last successful login.
Last login: Mon Aug 17 15:06:57 2020 from 192.168.2.62
Have a lot of fun...
suse64:~ # exit
logout
Connection to 192.168.2.90 closed.


````



## 	ssh-keygen

````
boscp08@boscp08-HP-Compaq-8510p:~$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/home/boscp08/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/boscp08/.ssh/id_rsa
Your public key has been saved in /home/boscp08/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:Xz2KHgD+gtbKj9tKAEIyHwrq9TrncYsMCvQ6TX4Xlt4 boscp08@boscp08-HP-Compaq-8510p
The key's randomart image is:
+---[RSA 3072]----+
|+..              |
|=+ .             |
|= ..  .          |
|o.. .. .     .   |
| o.  .. S   . o  |
|. .o.o = o o . . |
|. +=+o=.+ + .    |
|..o**=++.E .     |
| o. BB+.  .      |
+----[SHA256]-----+
boscp08@boscp08-HP-Compaq-8510p:~$ cd .ssh
boscp08@boscp08-HP-Compaq-8510p:~/.ssh$ ks
lks: command not found
boscp08@boscp08-HP-Compaq-8510p:~/.ssh$ ls
id_rsa  id_rsa.pub
boscp08@boscp08-HP-Compaq-8510p:~/.ssh$ cat id_rsa.pub 
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDmIvwY8gJrf601nii0W3e6zQoogKyhlpr9cWBfBMsN3qX2WT5RiYQlyP37yQ/o9OPOPsh0S/wZstg1o7UqGhJCkz0DFdKDSd+U0+jsdFZ836BsvOxynSI/r19hxMZJFcDD8R+QwZpeuCJw5JIeYFtuFDkAbH8wt3ug16w7uLpP4CpWvhjtP6wGMpd+z1NdcHVkcCaGyCwpCwb4JYPmb2Lv5ifq4cIDUK5qIs/XJ5Sr0M7dHPFNT/aNAZXLdfTsZCwf+AzNm2BS/rVbynRRuw3OoVzmHMVq4aLaZsEjSgtE0C5mMkHKo45yuU1fzbkEBzVVxyx02y4/anoGmGqKRWLIcXdZEj2YtNlm75dUcDsECxfU/dGMUA8neqZ98TMkChqyjmZkrNE2qv4i4c7bxMe5KJxjQfAUui2el1v2PC55QQKPqfn4Iw1RjiMlJ5P+sbnx5LUKFZH1vkt7aPCAjlDP7tg6YRGveP4BeyjFHKe8ePA8T4XLlqZ8KdEz50qA+zs= boscp08@boscp08-HP-Compaq-8510p

````


## 	20200827 /dev/sda5       466G   14G  429G   4% /


## sudo timeshift --create

````
boscp08@boscp08-HP-Compaq-8510p:~$ sudo timeshift --create
First run mode (config file not found)
Selected default snapshot type: RSYNC
Mounted '/dev/sda5' at '/run/timeshift/backup'
Selected default snapshot device: /dev/sda5
------------------------------------------------------------------------------
Estimating system size...
Creating new snapshot...(RSYNC)
Saving to device: /dev/sda5, mounted at path: /run/timeshift/backup
Synching files with rsync...
Created control file: /run/timeshift/backup/timeshift/snapshots/2020-08-27_10-06-04/info.json
RSYNC Snapshot saved successfully (124s)
Tagged snapshot '2020-08-27_10-06-04': ondemand
------------------------------------------------------------------------------
````

## sudo apt install timeshift

## sudo apt-get update && sudo apt-get upgrade -y

##	20200827 09:00 /dev/sda5	/dev/sda5 466G 7,1G 435G 2% /
