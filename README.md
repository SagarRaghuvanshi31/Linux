# Linux
Linux was developed by Linus Torvalds in 1991. <br>
Linux is an open source. <br>
Linux is free to use. <br>
Linux supports CLI and GUI. <br>
Linux is Multiuser, Multiprocessing and Multitasking. <br>
- **How to login Root user?** <br>
Alt+f2 = Search bar. <br>
Terminal name = gnome-terminal <br>
- **How to increase font size?** <br>
ctrl+shift++ add on + for increasing <br>
- **How to decrease font size?** <br>
ctrl + (-) <br>
- **For Multiple Tab** <br>
ctrl+shift+T
- **For Closing Tab** <br>
Alt+f4
### Basic Commands
- **Make a file** <br>
```
vi, vim, cat
```
- **Make a folder or directory** <br>
```
mkdir cloud
```
- **Make multiple directory** <br>
```
mkdir aws gcp azure
```
- **See the file and folder** <br>
```
ls (ls-listing) Blue = folder | Black, White, Green = file
```
- **Delete a folder** <br>
```
rmdir cloud
```
- **Delete a folder with data** <br>
```
rm -rf cloud (r = recursive, f = forecfully)
```
- **Remove multiple directory** <br>
```
rmdir aws gcp azure
```
- **See the data of file** <br>
```
cat asus
```
- **Delete a file without confirmation** <br>
```
rm -f asus (f = forcefully)
```
- **Delete a file with confirmation** <br>
```
rm hp (rm = remove)
```
- **Come to inside a folder** <br>
```
cd cloud (cd = change directory)
```
- **Make a sub folder** <br>
```
mkdir cloud - cd cloud  mkdir aa = bb cc
```
- **See the current location** <br>
```
pwd = present working directory
```
- **Go back 1 step** <br>
```
cd..
```
- **Go Back 2 step** <br>
```
cd../../..
```
- **Go back from all** <br>
```
cd
```
- **Add the data in file** <br>
```
cat > abc
Aws is a cloud
ctrl+d (for save and exit)
Echo 'azure is a cloud' >> abc
```
- **Copy a file** <br>
```
file aa(cloud) bb
cp aa bb
```
- **Copy a directory** <br>
```
test1/ aa bb cc  test2
cp -rvf test1/aa test2
cp -rvf test1/* test2
```
- **Cut Paste a file** <br>
```
mv = move
file = aws(cloud)  azure
mv -v aws  azure
```
- **Cut Paste a directory** <br>
```
11/aa bb cc   22
mv -v 11/aa  22
mv -v 11/*  22
```
- **Rename a filder/folder** <br>
```
mv oldname  newname
```
- **Make a hidden file** <br>
```
mkdir .aaa
cat..bbb
touch .ccc
```
- **See the hidden data** <br>
```
ls -a (a = archieve)
```
- **Add new user** <br>
```
adduser or useradd
```
- **Check current username** <br>
```
whoami or logname
```
- **See the hostname** <br>
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

**Ssh** = Secure Shell



