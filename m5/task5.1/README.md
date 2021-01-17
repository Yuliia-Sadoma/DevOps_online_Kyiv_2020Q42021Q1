# Module 5 

## Task 5.1

### PART 1.

1) Log in to the system as root.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/5.1.PNG?raw=true">

2) Using the passwd command to change the password. This command change the '/etc/shadow' file.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/2.PNG?raw=true">

3) Users registered in the system

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/33.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/34.PNG?raw=true">

4) Changing personal information.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/7.PNG?raw=true">

5) Example: Commands chfn -f and chfn -o.

Command chfn -f change the user's full name.

Command chfn -o change the user's other GECOS information.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/8.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/9.PNG?raw=true">

6) Viewing the contents of files .bash* using more command.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/10.PNG?raw=true">

7) Using the finger command.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/13.PNG?raw=true">

8) Listing the contents of the home directory.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/12.PNG?raw=true">

### PART 2.

1) Using "tree" command. 

- displaing all files that contain part "new"

- displaing all .txt files 

- list subdirectories of the root directory up to and including the second nesting level

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/14.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/15.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/16.PNG?raw=true">

2) Using command "file" to determine the type of file.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/17.PNG?raw=true">

3) Navigating the file system using "cd" command.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/18.PNG?raw=true">

4) Using "ls" command:

Command ls -l	shows list with long format.

Command ls -a	shows list all files including hidden file starting with '.'

Command ls -s	shows list file size

Command ls -ls shows list with long format with file size

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/19.PNG?raw=true">

5) Performing the following sequence of operations:

- creating a subdirectory in the home directory;

- creatinf a file containing information about directories located in the root directory (using I/O redirection operations);

- viewing the created file;

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/20.PNG?raw=true">

- copying the created file to your home directory using relative and absolute addressing.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/21.PNG?raw=true">

- deleting the previously created subdirectory with the file requesting removal;

- deleting the file copied to the home directory.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/22.PNG?raw=true">

6) Performing the following sequence of operations:

- creating a subdirectory test in the home directory;

- copying the .bash_history file to this directory while changing its name to labwork2;

- creating a hard and soft link to the labwork2 file in the test subdirectory;

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/23.PNG?raw=true">

- how to define soft and hard link, what do these concepts;

A symbolic or soft link is an actual link to the original file, whereas a hard link is a mirror copy of the original file.

- changing the data by opening a symbolic link. 

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/25.PNG?raw=true">

After I changed content of the main file changes were done only in labwork2 file and hard link file. This is because the hard disk is an exact copy of the main file, while the soft disk is an actual link to it. 

- renaming the hard link file to hard_lnk_labwork2;

- renaming the soft link file to symb_lnk_labwork2 file;

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/24.PNG?raw=true">

- deleting the labwork2. 

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/35.PNG?raw=true">


After deleting the labwork2 the soft link don't show any contents, while the hard link continues to work correctly. This is because the hard disk is an exact copy of the main file, while the soft disk is an actual link to it. 

7) Using the locate utility, all files that contain the squid and traceroute sequence where find.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/26.PNG?raw=true">

8-9) Determinating which partitions are mounted in the system and the types of these partitions. And counting the number of lines containing a given sequence of characters in a given file.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/27.PNG?raw=true">

10) Using the find command to find all files in the /etc directory containing the host character sequence.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/28.PNG?raw=true">

11) Listing all objects in /etc that contain the ss character sequence. Using find command and using grep.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/29.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/30.PNG?raw=true">

12) Organize a screen-by-screen print of the contents of the /etc directory.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/31.PNG?raw=true">

13) What are the types of devices and how to determine the type of device?

Few types of devices:

-Audio devices

-USB devices

-PCI devices

etc.

To determine the type of device you can use "ls -l /dev" command.

14) How to determine the type of file in the system, what types of files are there?

There are seven types of files:

|      -       | Regular File           |

|      d       | Directory              |

|      l       | Link File              |

|      c       | Character Device File  |

|      s       | Local Socket File      |

|      p       | Named Pipe File        |

|      b       | Block Device File      |

To determine the type of file in the system you can use 'ls -l' or 'file' commands.

15) Listing the first 5 directory files that were recently accessed in the /etc directory:

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.1/screenshots/32.PNG?raw=true">
