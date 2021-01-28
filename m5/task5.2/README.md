# Module 5 

## Task 5.2

1-4) The /etc/passwd file contains the following fields:

- User name

- Encrypted password

- User ID number

- User's group ID number 

- Full name of the user 

- User home directory

- Login shell

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/1.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/2.PNG?raw=true">

In the etc/passwd file we can find real users and pseudo-users or system users (such as daemon, bin, adm, nobody, man, sys, sshd). 

The /etc/group file contains the following fields:

- Group Name

- Group Password

- Group ID

- Group Members

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m1/task1.1/screenshots/3.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m1/task1.1/screenshots/4.PNG?raw=true">

UID - user ID number. Ranges: 0 for root, 1-999 and 65534 (nobody) for system users (pseudo-users), 1000 and above for regular users.

Using the id -u {UserNameHere} command we can get the real and effective user ID.

GID - user's group ID number

Using the id -g {UserNameHere} command we can get the real and effective group ID.

To find all the groups to which the user belongs we can use id -G {UserNameHere} command.

To view UID and all groups associated with username we can use the id {UserNameHere} command.

To view only the names of all groups associated with username, we can use the id -nG {UserNameHere} command.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/5.PNG?raw=true">

5) To add/create new user accounts we can use the useradd [OPTIONS] USERNAME command. Only root or users with sudo privileges can use the useradd command to create new user accounts.

In this command, we can use the following options: 

 -u - to create a User with Specific User ID

 -d - to create a User with Specific Home Directory

 -g - to create a User with Specific Group ID

 -G - to add a User to Multiple Groups

 -M - to add a User without Home Directory

 -e - to create a User with Account Expiry Date

 -c - to add a User with Custom Comments

 -s - to change User Login Shell

 -r - to create a System User

 etc.

 6) The "usermod -l login-name old-name" command change the name (account name) of an existing user from the old-name to login_name.

7) The /etc/skel directory contains files and directories that are automatically copied over to a new user's home directory when such user is created by the useradd command.

/etc/skel allows a system administrator to create a default home directory for all new users on a computer or network and thus to make certain that all users begin with the same settings or environment.

8)  userdel -r {UserNameHere}

The command remove the files in the user’s home directory along with the home directory itself and the user’s mail spool.

9) The simplest way to lock an account is with the passwd -l {UserNameHere} command or usermod -L {UserNameHere} command.

To to unlock an account we can use the passwd -u {UserNameHere} command or usermod -U {UserNameHere} command.

10) To remove a user's password we can use the passwd command with option -d (passwd -d {UserNameHere}). This option deletes the user password and makes the account password-less.

11) 

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/6.PNG?raw=true">

When y the extended format is used, we can see the following information about directory:

- The file type.

- The file permissions.

- Number of hard links to the file.

- File owner.

- File group.

- File size.

- Date and Time.

- File name.

12-14) 

Types of Users:

Owner: The user who creates the file or folder is the owner of that file or folder, denoted by ‘u’.

Group: When a user creates a file or folder, then other members of the group where the user belongs can access the file or folder. It is denoted by ‘g’.

Others/All: It indicates any user who is not the owner of a particular file or folder and does not belong to the file or folder owner’s group. ‘o’ is used to denote other users, and ‘a’ is used to denote all users.

Types of Permission:

Read: This permission is used to read any file or folder only. It is denoted by ‘r’ when it is defined by character, and it is denoted by 4 when it is defined by a number.

Write: This permission is used to write, append, or override any file or folder. It is denoted by ‘w’ and it is denoted by 2.

Execute: This permission is used to execute any file only. It is denoted by ‘x’ , and it is denoted by 1.

The chmod command is used to change the permission bits of the file or folder.

The chown command is used to change the ownership of user and group user for any file. 

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/7.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/8.PNG?raw=true">

15)

Permissions can also be represented numerically, using octal values (the digits from 0 to 7). 

When using octal numeric representation, certain numbers represent certain permissions, and these numbers are added or subtracted from each other to represent the final, combined permissions value. 

Specifically, the numbers 1, 2, and 4 represent the following permissions: 

- read denoted by 4

- write denoted by 2

- execute denoted by 1

For example, we can represent the symbolic permission of rwxrwxr-- using the three-digit octal number 774. The order of the digits is always the same: User, Group, Other.

In Linux, the default permissions value is 666 for a regular file, and 777 for a directory.

The umask command allows you to view or to set the file mode creation mask, which determines the permissions bits for newly created files or directories.

The default umask permissions for root user and remaining users are 0022 and 0002 respectively.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/11.PNG?raw=true">

16) 

 The sticky bit is working on the directory. If the sticky bit is set for a directory, all files in the directory can only be deleted or renamed by the owners of the files or by the root user. 

 For example, this is used in the /tmp directory, which acts as a recycle bin for temporary files.

 <img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/9.PNG?raw=true">

 chmod +t dir_name command to set sticky bit for the direcrory.

  <img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.2/screenshots/10.PNG?raw=true">

17) File should have -f attribute, which means that file exists and is a regular file. And also -x attribute, file should have execute permissions for owner, group and others.  
