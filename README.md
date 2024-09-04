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
- Linux is an open source. <br>
- Linux is free to use. <br>
- Linux supports CLI and GUI. <br>
- Linux is Multiuser, Multiprocessing and Multitasking. <br>

- **For Login Root user** <br>

  Alt+ctrl+t = Search bar <br>
  Terminal name = gnome-terminal <br>

- **To increase font size of Terminal** <br>
                                             
  ctrl+shift++ add on + for increasing <br>

- **To decrease font size of Terminal** <br>

  ctrl + (-) <br>

- **For Multiple Tab** <br>

  ctrl+shift+T

- **For Closing Tab** <br>

  Alt+f4

### Basic Commands

- **Make a file** <br>

Run this command to make a file

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

after the ls command you will see the output result <br>
blue colour = folder <br>
white, green colour = file
```
ls
```
```
ll
```

- **Delete a folder** <br>

Run this command to delete a folder

rmdir = remove directory <br>
cloud = folder name <br>
```
rmdir cloud
```

- **Delete a folder with data** <br>

Run this command to delete a folder with data <br>

rm = remove <br>
-rf = (-r = recursive, f = forcefully) <br>
cloud = folder name
```
rm -rf cloud (r = recursive, f = forecfully)
```
- **Remove multiple directory** <br>

Run this command to remove multiple directory

rmdir = remove directory <br>
aws gcp azure = directory name
```
rmdir aws gcp azure
```
- **See the data of file** <br>

Run this command to see tha data of that file 

cat = concatenate <br>
asus = file name
```
cat asus
```
- **Delete a file without confirmation** <br>

Run this command to delete a file without confirmation

rm = remove <br>
-f = forecully <br>
asus = file name
```
rm -f asus
```
- **Delete a file with confirmation** <br>

Run this command to delete a file with confirmation

rm = remove<br>
hp = file name
```
rm hp
```
- **Come to inside a folder** <br>

Run this command to come inside a folder

cd = change directory<br>
cloud = folder name <br>
```
cd cloud
```
- **Make a sub folder** <br>

Run this command to make a sub folder in a folder

make a mkdir cloud directory then use cd command to change directory into cloud after that make a folder of aa 

mkdir = make directory <br>
cloud = folder name <br>
cd cloud = change directory <br>
aa = sub folder
```
mkdir cloud - cd cloud  mkdir aa
```
- **See the current location** <br>

Run this command to see the present directory

pwd = present working directory
```
pwd 
```
- **Go back 1 step** <br>

Run this command to go back 1 step from folder/file

cd= change directory
```
cd..
```

- **Go back from all** <br>

Run this command to go back to the main page
```
cd
```
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
ctrl+d (for save and exit)
Echo 'azure is a cloud' >> abc
```
- **Copy a file** <br>

Run this command to copy a file

cp = copy
aa bb = file name
```
file aa bb
cp aa bb
```
- **Copy a directory** <br>

Run this command to copy a directory
```
test1/ aa bb cc  test2
cp -rvf test1/aa test2
cp -rvf test1/* test2
```
- **Cut Paste a file** <br>

Run this command to cut paste a file

mv = move
aws, azure = file name
-v = vervose
```
file = aws azure
mv -v aws  azure
```
- **Cut Paste a directory** <br>

Run this command to cut paste a directory
```
11/aa bb cc   22
mv -v 11/aa  22
mv -v 11/*  22
```
- **Rename a filder/folder** <br>

Run this command to rename a folder

mv = move
this command is use to move and rename
```
mv oldname  newname
```
- **Make a hidden file** <br>

Run this command to make a hidden file

mkdir = make directory
.aaa = hidden file

```
touch .aaa
```
- **See the hidden data** <br>

Run this command to see the hidden data

ls = listing
-a = archieve
```
ls -a
```
- **Add new user** <br>

Run this command to add a new user
```
adduser sagar <br>
useradd raghuvanshi
```
- **Check current username** <br>

Run this command to check current login username
```
whoami <br>
logname
```
- **See the hostname** <br>

Run this command to see the hostname
```
hostname or uname -n
```
- **Change the hostname temporary** <br>

Run this command to change hostname temporary
```
hostname sky
bash
```
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




