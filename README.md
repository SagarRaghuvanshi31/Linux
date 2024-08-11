# Linux

<img src="Linux.jpg"/>

## Table of Content

1. Introduction to Linux
2. For Login Root user
3. To increase font size of Terminal
4. To decrease font size of Terminal
5. For Multiple Tab
6. For Closing Tab
7. Basic Commands
8. File System Hierachy
9. User and Group Management
10. Permission
11. SSH
12. Apache
  
### Introduction to Linux 

- Linux was developed by Linus Torvalds in 1991. <br>
- Linux is an open source. <br>
- Linux is free to use. <br>
- Linux supports CLI and GUI. <br>
- Linux is Multiuser, Multiprocessing and Multitasking. <br>

- **For Login Root user** <br>

  Alt+ctrl+t = Search bar <br>
  Terminal name = gnome-terminal <br>

- **To increase font size of Terminal** <br>
                                             
  ctrl+shift++ add on + for increasing <br>

- **How to decrease font size of Terminal** <br>

  ctrl + (-) <br>

- **For Multiple Tab** <br>

  ctrl+shift+T

- **For Closing Tab** <br>

  Alt+f4

### Basic Commands

- **Make a file** <br>

This command is use to make a file

vi = visual editor, (vi) is a text editor <br>
vim = vi improved, it is a improved version of vi <br>
cat = concatenate, Display and create files <br>
touch (blue) = blue is a file name
```
touch blue
```
```
vi, vim, cat
```
- **Make a folder or directory** <br>

This command is use to make a folder <br>

mkdir = make directory <br>
cloud = folder name
```
mkdir cloud
```
- **Make multiple directory** <br>

This command is use to make multiple directory <br>
aws gcp azure = folders name
```
mkdir aws gcp azure
```
- **See the file and folder** <br>

This command is use to see the file and folder

ls = listing <br>
ll = long listing <br>

after the ls command you will see the output result <br>
blue colour = folder <br>
white, green colour = file
```
ls
```
```
ll
```
<img src="Screenshot from 2024-08-08 16-54-23.png"/>

- **Delete a folder** <br>

This command is use to delete a folder

rmdir = remove directory <br>
cloud = folder name <br>
```
rmdir cloud
```
<img src="Screenshot from 2024-08-08 17-40-18.png"/>

- **Delete a folder with data** <br>

This command is use to delete a folder with data <br>

rm = remove <br>
-rf = (-r = recursive, f = forcefully) <br>
cloud = folder name
```
rm -rf cloud (r = recursive, f = forecfully)
```
- **Remove multiple directory** <br>

this command is use to remove multiple directory

rmdir = remove directory <br>
aws gcp azure = directory name
```
rmdir aws gcp azure
```
- **See the data of file** <br>

this command is use to see tha data of that file 

cat = concatenate <br>
asus = file name
```
cat asus
```
- **Delete a file without confirmation** <br>

this command is use to delete a file without confirmation

rm = remove <br>
-f = forecully <br>
asus = file name
```
rm -f asus
```
- **Delete a file with confirmation** <br>

this command is use to delete a file with confirmation

rm = remove<br>
hp = file name
```
rm hp
```
- **Come to inside a folder** <br>

this command is use to come inside a folder

cd = change directory<br>
cloud = folder name <br>
```
cd cloud
```
- **Make a sub folder** <br>

this command is use to make a sub folder in a folder

make a mkdir cloud directory then use cd command to change directory into cloud after that make a folder of aa 

mkdir = make directory <br>
cloud = folder name <br>
cd cloud = change directory <br>
aa = sub folder
```
mkdir cloud - cd cloud  mkdir aa
```
- **See the current location** <br>

this command is use to see the present directory

pwd = present working directory
```
pwd 
```
- **Go back 1 step** <br>

thsi command is use to go back 1 step from folder/file

cd= change directory
```
cd..
```

- **Go back from all** <br>

this command is use to go back to the main page
```
cd
```
- **Add the data in file** <br>

this command is use to add data in a file

cat = concatenate <br>
abc = file name <br>
Aws is a cloud = data that we were adding <br>
ctrl+d = for save and exit <br>
Echo = to display text
```
cat > abc
Aws is a cloud
ctrl+d (for save and exit)
Echo 'azure is a cloud' >> abc
```
- **Copy a file** <br>

this command is use to copy a file

cp = copy
aa bb = file name
```
file aa bb
cp aa bb
```
- **Copy a directory** <br>

this command is use to copy a directory
```
test1/ aa bb cc  test2
cp -rvf test1/aa test2
cp -rvf test1/* test2
```
- **Cut Paste a file** <br>

this command is use to cut paste a file

mv = move
aws, azure = file name
-v = vervose
```
file = aws azure
mv -v aws  azure
```
- **Cut Paste a directory** <br>

this command is use to cut paste a directory
```
11/aa bb cc   22
mv -v 11/aa  22
mv -v 11/*  22
```
- **Rename a filder/folder** <br>

this command is use to rename a folder

mv = move
this command is use to move and rename
```
mv oldname  newname
```
- **Make a hidden file** <br>

this command is used to make a hidden file

mkdir = make directory
.aaa = hidden file

```
touch .aaa
```
- **See the hidden data** <br>

this command is use to see the hidden data

ls = listing
-a = archieve
```
ls -a
```
- **Add new user** <br>

this command is use to add a new user
```
adduser sagar <br>
useradd raghuvanshi
```
- **Check current username** <br>

this command is use to check current login username
```
whoami <br>
logname
```
- **See the hostname** <br>

this command is used to see the hostname
```
hostname or uname -n
```
- **Change the hostname temporary** <br>
```
hostname sky
bash
```
- **Change the name permanently** <br>
```
nmtui = network manager terminal user interface
bash
```
- **See the all info** <br>
```
uname -a
```
- **See the date and time** <br>
```
date
```
- **Change the date and time** <br>
```
date -s "2 jan 2050 18:30:45"
```
- **Shutdown the server** <br>
```
init 0 or shutdown -p or poweroff
```
- **Restart the Server** <br>
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
**Give the Password** <br>
```
passwd harsh <br>
```
**Make a user without password** <br>
```
passwd -d harsh (d = delete)
```
**Delete the user but keep data** <br>
```
userdel harsh <br>
```
**Delete the user with data** <br>
```
userdel -r test (r = recursive) <br>
```

### User modification
**Change the login name** <br>
```
usermod -l newname oldname (l = loginname) <br>
```
**Change UID** <br>
```
usermod -u 2000 name (u = uid) <br>
```
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
groupadd HR <br>
```
**Delete the secondary group** <br>
```
groupdel HR 
vim /etc/group <br>
```

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
 adduser aa
 chmod 777 aa
```

### SSH

**Ssh** = Secure Shell <br>
it is a protocol which is use to take the console of linux remotly. it's port no. is 22. <br>
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




