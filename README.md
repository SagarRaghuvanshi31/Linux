# Linux

<img src="Linux.jpg"/>

## Table of Content

1. [Introduction to Linux](#Introduction-to-Linux)
2. [To Login Root user](#For-Login-Root-user)
3. [To increase font size of Terminal](#To-increase-font-size-of-Terminal)
4. [To decrease font size of Terminal](#To-decrease-font-size-of-Terminal)
5. [For Multiple Tab](#For-Multiple-Tab)
6. [For Closing Tab](#For-Closing-Tab)
7. [Basic Commands](#Basic-Commands)
8. [File System Hierachy](#File-System-Hierachy)
9. [User and Group Management](#User-and-Group-Management)
10. [Permission](#Permission)
11. [SSH](#SSH)
12. [Apache](#Apache)
  
### Introduction to Linux 

- Linux was developed by Linus Torvalds in 1991. <br>
- Linux is open source. <br>
- Linux is free to use. <br>
- Linux supports CLI and GUI. <br>
- Linux is multiuser, multiprocessing and multitasking. <br>

### To install Ubuntu

- **Version** <br>

Ubuntu 22.04.4 LTS

1. Visit Ubuntu’s official website: https://ubuntu.com/ <br>
Download the latest LTS (long-term support) for the computer's system (usually 64-bit). <br>

2. Create a Bootable USB Drive: <br>
Use a tool like Rufus, Etcher, or Unetbootin to create a bootable USB drive from the downloaded ISO. <br>

3. Boot from the USB Drive: <br>
Restart the computer and enter the BIOS or UEFI settings. <br>
Find the options for boot order and set the USB drive as the most important. <br>
Save the changes and exit. <br>

4. Launch the Ubuntu installer: <br>
Once your computer boots from the USB drive, you will see the Ubuntu installer. <br>
Select your language and click "Install Ubuntu." <br>

5. Select the installation type: <br>
Decide how you want to install Ubuntu: <br>
Normal Installation: Ubuntu will replace your current operating system. <br>
Wipe the disk and install Ubuntu: This will wipe all the data on your hard drive and install Ubuntu. <br>
Something else: This program allows you to manually partition your hard drive and add Ubuntu to other operating systems. <br>

6. Choose your time zone and keyboard layout: <br>
Select location and keyboard layout. <br>

7. Create a user account: <br>
Enter your username, username, and password. <br>

8. Start the installation: <br>
Click "Install Now" to start the installation process. <br>

9. Restart your computer: <br>
Once the installation is complete, your computer will restart.


- **To Login Root user** <br>

  Alt+Ctrl+T = Open terminal <br>
  
  Terminal name = gnome-terminal <br>

- **To increase font size of Terminal** <br>

'+' = to increase font size of terminal
                                             
  Ctrl+Shift ++ add on + for increasing <br>

- **To decrease font size of Terminal** <br>

  ctrl + '-' <br>

- **For Multiple Tab** <br>

  ctrl+shift+T

- **For Closing Tab** <br>

  Alt+F4

### Basic Commands

- **Make a file** <br>

Run this command to make a file

vi = visual editor, (vi) is a text editor <br>
vim = vi improved, it is a improved version of vi <br>
cat = Concatenate, Display and create files <br>
blue = blue is a file name

```
touch blue
```
```
vi, vim, cat
```
- **Make a folder or directory** <br>

Run this command to make a folder <br>

mkdir = make directory <br>
cloud = folder name
```
mkdir cloud
```
- **Make multiple directory** <br>

Run this command to make multiple directory <br>

aws gcp azure = folders name

```
mkdir aws gcp azure
```
- **See the file and folder** <br>

Run this command to see the file and folder

ls = listing <br>
ll = long listing <br>

after ls command you will see the output result <br>
blue colour = folder <br>
white, green colour = file

```
ls
```
```
ll
```

**Output** <br>
root@sagar:~ # touch blue <br>
root@sagar:~ # mkdir cloud <br>
root@sagar:~ # mkdir aws gcp azure <br>
root@sagar:~ # ls <br>
aa  agg  aw  aws  azure  blue  cloud  gcp  rahul  snap  software


- **Delete a folder** <br>

Run this command to delete a folder

rmdir = remove directory <br>
cloud = folder name <br>

```
rmdir cloud
```

**Output**
root@sagar:~ # rmdir cloud <br>
root@sagar:~ # ls <br>
aa  agg  aw  aws  azure  blue  gcp  rahul  snap  software


- **Delete a folder with data** <br>

Run this command to delete a folder with data <br>

rm = remove <br>
-rf = (-r = recursive, f = forcefully) <br>
cloud = folder name

```
rm -rf cloud
```

**Output** <br>
rm -rf cloud <br>
root@sagar:~ # ls <br>
aa  agg  aw  blue  rahul  snap  software

- **Remove multiple directory** <br>

Run this command to remove multiple directory

rmdir = remove directory <br>
aws gcp azure = directory name

```
rmdir aws gcp azure
```

**Output**
root@sagar:~ # rmdir aws gcp azure <br>
root@sagar:~ # ls <br>
aa  agg  aw  blue  rahul  snap  software

- **See the data of file** <br>

Run this command to see tha data of that file 

cat = concatenate <br>
asus = file name

```
cat asus
```

**Output** <br>
root@sagar:~ # vi asus <br>
root@sagar:~ # cat asus <br>
abc <br>
is am are

- **Delete a file without confirmation** <br>

Run this command to delete a file without confirmation

rm = remove <br>
-f = forecully <br>
asus = file sky

```
rm -f sky
```

**Output** <br>
root@sagar:~ # touch sky <br>
root@sagar:~ # ls <br>
aa  agg  asus  aw  blue  rahul  sky  snap  software <br>
root@sagar:~ # rm sky <br>
root@sagar:~ # ls <br>
aa  agg  asus  aw  blue  rahul  snap  software

- **Come to inside a folder** <br>

Run this command to come inside a folder

cd = change directory<br>
cloud = folder name <br>

```
mkdir cloud
cd cloud
```

**Output** <br>
root@sagar:~ # mkdir cloud <br>
root@sagar:~ # cd cloud <br>
root@sagar:~ /cloud #

- **See the current location** <br>

Run this command to see the present directory

pwd = present working directory

```
pwd 
```

**Output**
root@sagar:~ # pwd <br>
/root

- **Go back 1 step** <br>

Run this command to go back 1 step from folder/file

cd= change directory

```
cd ..
```

**Output**
root@sagar:~ /cloud/ad/dc# cd ..  <br>
root@sagar:~ /cloud/ad# 

- **Go back from all** <br>

Run this command to go back to the main page

```
cd
```

**Output**
root@sagar:~ /cloud/ad/dc# cd <br>
root@sagar:~ # 

- **Add the data in file** <br>

Run this command to add data in a file

cat = concatenate <br>
abc = file name <br>
Aws is a cloud = data that we were adding <br>
ctrl+d = for save and exit <br>
Echo = to display text

```
cat > abc
Aws is a cloud
ctrl+d 
Echo 'azure is a cloud' >> abc
```

**Output**
sagar@sagar:~ $ cat > abc <br>
aws is a cloud <br>
sagar@sagar:~ $ cat abc <br>
aws is a cloud <br>
sagar@sagar:~ $ echo 'azure is a cloud' >> abc <br>
sagar@sagar:~ $ cat abc <br>
aws is a cloud <br>
azure is a cloud

- **Copy a file** <br>

Run this command to copy a file

cp = copy <br>
aa bb = file name

```
file aa bb
cp aa bb
```

**Output**
sagar@sagar:~ $ cat > aa <br>
1234 <br>
sagar@sagar:~ $ cp aa bb <br>
sagar@sagar:~ $ cat bb <br>
1234

- **Copy a directory** <br>

Run this command to copy a directory

cp = copy <br>
-rvf = recursive, verbose, forcefully

```
test1/ aa bb cc  test2
cp -rvf test1/aa test
```

**Output**
sagar@sagar:~ $ test1/ aa bb cc  test2 <br>
sagar@sagar:~ $ cp -rvf test1/* test2 <br>
sagar@sagar:~ $ test1  test2/aa bb cc

- **Cut Paste a file** <br>

Run this command to cut paste a file

mv = move
aws, azure = file name
-v = vervose

```
mv -v aws  azure
```

**Output**
root@sky:~ # touch aws azure <br>
root@sky:~ # mv -v aws azure  <br>
renamed 'aws' -> 'azure'  <br>
root@sky:~ # ls  <br>
abc  asus  azure  black  cc  cloud  mkdir  snap  <br>
aa  agg  aw    bb     blue   cd  light  rahul  software

- **Cut Paste a directory** <br>

Run this command to cut paste a directory

```
11/aa bb cc   22
mv -v 11/aa  22
mv -v 11/*  22
```

**Output**
root@sky:~ # mv -v 11/ dd 22  <br>
renamed '11/' -> '22/11'  <br>
renamed 'dd' -> '22/dd' v
root@sky:~ # ls  <br>
abc  asus  azure  blue  cloud  light  rahul  software  <br>
22  agg  aw    black  cd    ee     mkdir  snap

- **Rename a filder/folder** <br>

Run this command to rename a folder

mv = move  <br>
this command is use to move and rename

```
mv oldname  newname
```

**Output**
root@sky:~ # touch oldname <br>
root@sky:~ # mv oldname newname  <br>
root@sky:~ # ls  <br>
abc  asus  azure  blue  cloud  light  newname  snap  <br>
22  agg  aw    black  cd    ee     mkdir  rahul    software

- **Make a hidden file** <br>

Run this command to make a hidden file

mkdir = make directory  <br>
.aaa = hidden file

```
touch .aaa
```
- **See the hidden data** <br>

Run this command to see the hidden data

ls = listing  <br>
-a = archieve

```
ls -a
```

**Output**
sagar@sagar:~ $ touch .aaa  <br>
sagar@sagar:~ $ ls  <br>
 aws     Desktop     mouse.py   __pycache__       Untitled1.ipynb   web
'='    azure   Documents   Music      PycharmProjects   Untitled.ipynb
 aa    bb      Downloads   myenv      snap              untitled.py
 aaa   blue    gcp         np         Templates         util.py
 abc   cc      Linux       Pictures   test1             venv

sagar@sagar:~ $ ls -a  <br>
aa              .gnupg               snap
 .aaa            .gphoto              .ssh
 aaa             .idea                .sudo_as_admin_successful
 abc             .ipynb_checkpoints   Templates
 asd             .ipython             test1
 aws             .java                test2
 
- **Add new user** <br>

Run this command to add a new user

```
adduser raghuvanshi 
```

**Output**
root@sagar:~ # adduser raghuvanshi  <br>
root@sagar:~ # getent passwd raghuvanshi  <br>
raghuvanshi:x:1003:1004:,,,:/home/raghuvanshi:/bin/bash

- **Check current username** <br>

Run this command to check current login username

```
whoami 
```

**Output**
root@sagar:~ # whoami
root

- **See the hostname** <br>

Run this command to see the hostname

```
hostname or uname -n
```

**Output**
sagar@sagar:~ $ uname -n <br>
sagar <br>
sagar@sagar:~ $ hostname <br>
sagar

- **Change the hostname temporary** <br>

Run this command to change hostname temporary

```
hostname sky
bash
```

**Output**
root@sagar:~ # hostname sky <br>
root@sagar:~ # bash  <br>
root@sky:~ #

- **Change the name permanently** <br>

Run this command to change permanentaly

nmtui = network manager terminal user interface <br>
bash = Bourne Again SHell

```
nmtui
bash
```
- **See the all info** <br>

Run this command to all system info

uname = Unix name <br>
-a = all

```
uname -a
```

**Output**
root@sky:~ # uname -a  <br>
Linux sky 6.8.0-40-generic #40~22.04.3-Ubuntu SMP PREEMPT_DYNAMIC Tue Jul 30 17:30:19 UTC 2 x86_64 x86_64 x86_64 GNU/Linux

- **See the date and time** <br>

Run this command to see date and time

```
date
```
- **Change the date and time** <br>

Run this command to change date and time

```
date -s "2 jan 2050 18:30:45"
```

**Output**
root@sky:~ # date  <br>
Wednesday 04 September 2024 10:28:53 PM IST

- **Shutdown the server** <br>

Run this command to shutdown the server

```
init 0 or shutdown -p or poweroff
```
- **Restart the Server** <br>

Run this command to restart the server

```
init 6 or reboot or shutdown -r
```
### File System Hierachy

**/ root** = home directory of root user <br>

**/ boot** = booting file <br>

**/ home** = privilege and non-privilege <br>

**/ dev(device)** = contain hardware file <br>

**/ bin(binaries)** = contain command file which can run by root and non-privilege <br>

**/ sbin(super binaries)** = contain command file which can run by only root (init0, init6) <br>

**/ etc** = contain server configuration file and system configuration file (user, group file, password) <br>

**/ lib** = save OS configuration files <br>

**/ mnt** = use to mounting <br>

### User and Group Management <br>

**User** = who use the system <br>

**Linux** = Types of user <br>

- **Privilege user** = full power <br>

- **Non-Privilege user** = less power <br>

- **System user** = automatically make <br>

kernal not understand the username, it understand ID (UID = user identification)

- **Privilege user** = RHEL 5,6,7,8,9 = UID = 0
- 
- **Non-Privilege user** = RHEL 5,6 = 500 or above
- 
- **System user** = RHEL 5,6 = 1-499, RHEL 7,8,9 = 1-999

### User Management

**Make a user** <br>

```
useradd harsh or adduser harsh
```
**To list user** <br>

cat = concatenate <br>
grep = Global Regular Expression Print, Searches text for patterns and prints lines that match.
```
cat /etc/passwd | grep harsh
```
**Output**
root@sagar:~ # cat /etc/passwd | grep harsh <br>
harsh:x:1003:1003::/home/harsh:/bin/sh

**Give the Password** <br>

```
passwd harsh
```

**Output** <br>
root@sagar:~ # passwd harsh <br>
New password: <br>
BAD PASSWORD: The password is shorter than 8 characters <br>
Retype new password: <br>
passwd: password updated successfully 

**Delete the user but keep data** <br>

```
userdel harsh 
```
**Delete the user with data** <br>

```
userdel -r test 
```

### User modification

**Change the login name** <br>

l = login name
```
usermod -l vivek harsh
```

**Output** <br>
root@sagar:~ # usermod -l vivek harsh <br>
vivek:x:1003:1003::/home/harsh:/bin/sh 

**Change UID** <br>

```
usermod -u 2000 vivek (u = uid) 
```

**Output** <br>
root@sagar:~ # cat /etc/passwd | grep vivek <br>
vivek:x:1003:1003::/home/harsh:/bin/sh

root@sagar:~ # usermod -u 2000 vivek usermod -u 2000

root@sagar:~# cat /etc/passwd | grep vivek <br>
vivek:x:2000:1003::/home/harsh:/bin/sh

**Give the comment** <br>

```
usermod -c "IT ADMIN" username (c = comment) 
```

**Change the home directory** <br>

```
mkdir /data
chmod 777 /data = change permission 
usermod -d /data name (d = directory)
```

### Group Management

**Group** = collection of users <br>

**Types of group**

- **Primary Group** = automatically make <br>

- **Secondary Group** = we have to make <br>

**Make a secondary group** <br>

```
groupadd hr
```
**To check added group** <br>

```
getent group hr
```

**Output**
root@sky:~ # groupadd hr  <br>
root@sky:~ # getent group hr  <br>
hr:x:1006:

**Delete the secondary group** <br>

```
groupdel hr 
vim /etc/group 
```

**Output** <br>
root@sagar:~ # groupadd hr <br>
root@sagar:~ # getent group hr  <br>
hr:x:1003:  <br>
root@sagar:~ # groupdel hr <br>
root@sagar:~ # getent group hr <br>


### Permission

**See the Permission** <br>
drwxr-xr-x . 2 root root 6jan 10:40:00 azure <br>
rwxr-xr-x = permission <br>
. = ACL <br>
2 = Subfolder <br>
root = owner <br>
6 = size in byte <br>
jan 1:40:00 = date and time <br>
azure = name <br>

**Types of Permission**

- **Read** = read the data = r <br>

- **Write** = edit the data = w <br>

- **Execute** = come to inside the folder, file = x <br>

- **No Permission** = -

**User** <br>

- **Privilege** = rwx <br>

- **Non-Privilege** = r-w <br>

- **System User** = r-x <br>

**Change the Permission** <br>

 **chmod** = for changing permission
 (777 = Full permission)
```
 touch aa
 chmod 777 aa
```

**Output**
  
root@sagar:~ # touch aa <br>
root@sagar:~ # ls -l aa <br>
-rw-r--r-- 1 root root 0 Sep  4 20:00 aa <br>
root@sagar:~ # chmod 777 aa <br>
root@sagar:~ # ls -l aa <br>
-rwxrwxrwx 1 root root 0 Sep  4 20:00 aa


### SSH

**Ssh** = Secure Shell <br>

It is a protocol which is use to take the console of linux remotly. <br>

It's port no. is 22. <br>

SSH encrypts the data being sent, providing secure communication over unsecured networks. <br>

It’s used primarily for remote login, file transfers and executing commands on remote servers. <br>


**service** = sshd (secure shell domain) <br>

**To install the SSH client and server**

```
sudo apt update
sudo apt install openssh-client openssh-server
```

**Start and enable the SSH server to run on boot**

```
sudo systemctl start ssh
sudo systemctl enable ssh
```

**Check the status of the SSH server to confirm it's running**

```
sudo systemctl status ssh
```

**Configuration file** 

```
/etc/ssh/sshd_config 
```
**log file**  

```
/var/log/secure 
```

### LVM

Logical Volume Manager (LVM) allows users to abstract and manage disk space more efficiently than traditional partitioning methods.

LVM enables the creation of logical volumes that can span across multiple physical devices, providing more flexibility in disk management.

**LVM Components**

Physical Volume (PV): The physical storage devices (like hard drives, SSDs, etc.) that are used in LVM.

Volume Group (VG): A collection of physical volumes combined into a single logical pool of storage.

Logical Volume (LV): A virtual partition created from the volume group. LVs behave like regular partitions but are more flexible.

**Create Physical Volumes**

First, initialize one or more partitions or disks as PVs.

/dev/sdb is a new disk, initialize it as a physical volume.

```
sudo pvcreate /dev/sdb
```

**To view existing physical volumes**

```
sudo pvs
```

**Create a Volume Group**

Combine one or more PVs into a VG.
Create a VG named vg_data using /dev/sdb

```
sudo vgcreate vg_data /dev/sdb
```

**To view all volume groups**

```
sudo vgs
```

 **Create Logical Volumes**

From the VG, create LVs which will act as storage partitions.

Create a 10GB LV called lv_data from vg_data.

```
sudo lvcreate -L 10G -n lv_data vg_data
```

**To view all logical volumes**

```
sudo lvs
```

**List active LVM volumes**

```
lvscan
```

**Remove a logical volume**

```
lvremove /dev/vg_name/lv_name
```

**Remove a volume group**

```
vgremove vg_name
```

### Cronjob.

A cron job is a scheduled task in Unix-like operating systems that automates repetitive tasks at specified times or intervals. <br>

The cron daemon is a background service that runs the scheduled tasks at their defined times.

Crontab is the file where you define cron jobs. Each user can have their own crontab, or there can be a system-wide crontab.

Use crontab -e to edit the crontab file and define your cron jobs.

**Here's what an asterisk (*) means in each field of the cron schedule**

Minute: * in the minute field means "every minute."

Example: * 5 * * * - Runs every minute during the 5th hour (5:00 AM - 5:59 AM).
Hour: * in the hour field means "every hour."

Example: 0 * * * * - Runs at the start of every hour (e.g., 1:00, 2:00, etc.).
Day of Month: * in the day-of-month field means "every day of the month."

Example: 0 0 * * * - Runs at midnight every day.
Month: * in the month field means "every month."

Example: 0 0 1 * * - Runs at midnight on the first day of every month.
Day of Week: * in the day-of-week field means "every day of the week."

Example: 0 0 * * * - Runs at midnight every day.

**To Setting up Crontab**

e = edit crontab file

```
crontab -e
```

**Viewing Scheduled Jobs**

l = list

```
crontab -l
```

### Nginx

Nginx is a high-performance HTTP and reverse proxy server, widely used for serving web content and handling high loads.

It can distribute incoming traffic across multiple servers, improving performance and reliability.

Nginx can act as an intermediary between clients and backend servers, hiding the backend structure and distributing requests.

Commonly used for hosting websites, acting as a gateway for APIs, managing microservices, and improving the performance of high-traffic applications.

**To install Nginx**

```
sudo apt update
sudo apt install nginx
```

**After installation, start the Nginx service**

```
sudo systemctl start nginx
```

**To enable Nginx to start on boot**

```
sudo systemctl enable nginx
```

**Basic Configuration file**

```
/etc/nginx/nginx.conf
```

**To edit the configuration**

```
sudo nano /etc/nginx/nginx.conf
```

### HAProxy

HAProxy (High Availability Proxy) is an open-source, high-performance load balancer and reverse proxy.

Commonly used for distributing traffic across web servers to ensure high availability, reliability, and scalability.

**Installing HAProxy**

```
sudo apt update
sudo apt install haproxy
```

**After installation, you can check the HAProxy version to ensure it was installed correctly**

```
haproxy -v
```

**To start HAProxy after configuration**

```
sudo systemctl start haproxy
```

**To enable HAProxy to start on boot**

```
sudo systemctl enable haproxy
```

**To check the status**

```
sudo systemctl status haproxy
```

**Basic Configuration File**

```
/etc/haproxy/haproxy.cfg
```

**To edit configuration file**

```
sudo nano /etc/haproxy/haproxy.cfg
```
