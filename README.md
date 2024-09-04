# Linux

<img src="Linux.jpg"/>

## Table of Content

1. [Introduction to Linux](#Introduction-to-Linux)
2. [For Login Root user](#For-Login-Root-user)
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


- **For Login Root user** <br>

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
adduser raghuvanshi <br>
```

**Output**
root@sagar:~ # adduser raghuvanshi  <br>
root@sagar:~ # getent passwd raghuvanshi  <br>
raghuvanshi:x:1003:1004:,,,:/home/raghuvanshi:/bin/bash

- **Check current username** <br>

Run this command to check current login username
```
whoami <br>
logname
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
-a = archieve
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

**/ var(variables)** = contains server log, database file <br>

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
- **Non-Privilege user** = RHEL 5,6 = 500 or above
- **System user** = RHEL 5,6 = 1-499, RHEL 7,8,9 = 1-999

### User Management
**Make a user** <br>
```
useradd harsh or adduser harsh <br>
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
passwd harsh <br>
```

**Output** <br>
root@sagar:~ # passwd harsh <br>
New password: <br>
BAD PASSWORD: The password is shorter than 8 characters <br>
Retype new password: <br>
passwd: password updated successfully 

**Delete the user but keep data** <br>
```
userdel harsh <br>
```
**Delete the user with data** <br>
```
userdel -r test 
```

### User modification
**Change the login name** <br>
l = login name <br>
```
usermod -l vivek harsh
```

**Output** <br>
root@sagar:~ # usermod -l vivek harsh <br>
vivek:x:1003:1003::/home/harsh:/bin/sh 

**Change UID** <br>
```
usermod -u 2000 vivek (u = uid) <br>
```

**Output** <br>
root@sagar:~ # cat /etc/passwd | grep vivek <br>
vivek:x:1003:1003::/home/harsh:/bin/sh

root@sagar:~ # usermod -u 2000 vivek usermod -u 2000

root@sagar:~# cat /etc/passwd | grep vivek <br>
vivek:x:2000:1003::/home/harsh:/bin/sh

**Give the comment** <br>
```
usermod -c "IT ADMIN" username (c = comment) <br>
```
**Change the home directory** <br>
```
mkdir /data <br>
chmod 777 /data = change permission <br>
usermod -d /data name (d = directory)
```

### Group Management
**Group** = collection of users <br>

**Types of group**
- **Primary Group** = automatically make <br>
- **Secondary Group** = we have to make <br>

**Make a secondary group** <br>
```
groupadd hr <br>
```
**To check added group** <br>
```
getent group hr
```

**Output**
root@sky:~ # groupadd hr
root@sky:~ # getent group hr
hr:x:1006:

**Delete the secondary group** <br>
```
groupdel hr 
vim /etc/group <br>
```

**Output** <br>
root@sagar:~ # groupadd hr <br>
root@sagar:~ # getent group hr
hr:x:1003:
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
it is a protocol which is use to take the console of linux remotly. <br>
it's port no. is 22. <br>
**service** = sshd (secure shell domain) <br>

**Configuration file** 
```
/etc/ssh/sshd_config <br>
```
**log file**  
```
/var/log/secure <br>
```

### Apache
It is use to execute/run website <br>
It is also called webserver <br>

**2 Protocol** <br>

**http** = hyper text transfer protocol <br>
**port no** = 80 <br>

**https** = hyper text transfer protocol secure <br>
**port no** = 443 <br>

**service** 
```
httpd demon
```
**package name** 
```
httpd
```
**configuration file** 
```
/etc/httpd/conf/httpd.conf
```




