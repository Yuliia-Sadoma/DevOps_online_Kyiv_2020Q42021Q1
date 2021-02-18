# Module 5

## TASK5.3

### Part1

1) How many states could has a process in Linux?

Process in Linux could have six following states:

-created

-ready

-running

-terminated

-waiting

-zombie

2) Examine the pstree command. Make output (highlight) the chain (ancestors) of the current
process.

Pstree is a Linux command that shows the running processes as a tree. It is used as a more visual alternative to the ps command.

"pstree -p" -  to display PIDs.

"pstree -p" -  to include command line arguments in output.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/1.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/3.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/2.PNG?raw=true">


3) What is a proc file system?

Proc file system (procfs) is virtual file system created on fly when system boots and is dissolved at time of system shut down. It contains the useful information about the processes that are currently running, it is regarded as control and information centre for kernel.

4) Print information about the processor (its type, supported technologies, etc.).

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/4.PNG?raw=true">


5) Use the ps command to get information about the process. The information should be as
follows: the owner of the process, the arguments with which the process was launched for
execution, the group owner of this process, etc.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/5.PNG?raw=true">

6) How to define kernel processes and user processes?

User-space processes have its own virtual address space. Kernel processes or threads do not have their own address space, they operate within kernel address space only. And they may be started before the kernel has started any user process (e.g. init).

7) Print the list of processes to the terminal. Briefly describe the statuses of the processes.
What condition are they in, or can they be arriving in?

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/7.PNG?raw=true">

R - running or runnable (on run queue)

S - interruptible sleep (waiting for an event to complete)

T - stopped by job control signal

t - stopped by debugger during the tracing

W - paging (not valid since the 2.6.xx kernel)

X - dead (should never be seen)

Z - defunct ("zombie") process, terminated but not reaped by its parent

< - high-priority (not nice to other users)

N - low-priority (nice to other users)

L - has pages locked into memory (for real-time and custom IO)

s - is a session leader

l - is multi-threaded (using CLONE_THREAD, like NPTL pthreads do)

+ - is in the foreground process group

8) Display only the processes of a specific user.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/6.PNG?raw=true">

9) What utilities can be used to analyze existing running tasks (by analyzing the help for the ps
command)?

The ps command, short for Process Status, is a command line utility that is used to display or view information related to the processes running in a Linux system.

10) What information does top command display?

Top command is used to show the Linux processes. It provides a dynamic real-time view of the running system. Usually, this command shows the summary information of the system and the list of processes or threads which are currently managed by the Linux Kernel.

11) Display the processes of the specific user using the top command.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/8.PNG?raw=true">

12) What interactive commands can be used to control the top command? Give a couple of
examples.

-‘u‘ option will display specific User process details

-(Shift+O) to sort field via field letter, for example press ‘a‘ letter to sort process with PID (Process ID)

-‘c‘ option in running top command, it will display absolute path of running process

-(Shift+P) to sort processes as per CPU utilization. See screenshot below

-‘z‘ option in running top command will display running process in color which may help you to identified running process easily

-‘h‘ option to obtain the top command help

-‘r‘ option to change the priority of the process also called Renice

-(Shift+M) to sort processes by usage Memmory

-(Shift+T) to sort processes by Time of process

13) Sort the contents of the processes window using various parameters (for example, the
amount of processor time taken up, etc.)

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/11.PNG?raw=true">

-(Shift+M) to sort processes by usage Memmory

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/12.PNG?raw=true">

-(Shift+T) to sort processes by Time of process

14) Concept of priority, what commands are used to set priority?

Nice command is used to run a process with an user defined priority whereas renice command is used to change the priority of a running process. Generally, nice and renice commands are used to change the priority than the default priority of a process.

15) Can I change the priority of a process using the top command? If so, how?

Once given top command, press r. Give PID value of the process you want to change the process value. Give renice value (from -20 to +19)

relation between nice value and priority is :

PR = NI + 20

16) Examine the kill command. How to send with the kill command process control signal? Give an example of commonly used signals.

Kill command in Linux (located in /bin/kill), is a built-in command which is used to terminate processes manually. kill command sends a signal to a process which terminates the process. If the user doesn’t specify any signal which is to be sent along with kill command then default TERM signal is sent that terminates the process.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/10.PNG?raw=true">

17) Commands jobs, fg, bg, nohup. What are they for? Use the sleep, yes command to
demonstrate the process control mechanism with fg, bg.

Process control commands in Unix are:

bg - put suspended process into background

fg - bring process into foreground

jobs - list processes

Nohup, short for no hang up is a command in Linux systems that keep processes running even after exiting the shell or terminal.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/9.PNG?raw=true">

### Part2

SSH connection to host

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/13.PNG?raw=true">

Implementing 3 different keys for encryption in SSH:

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/14.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/15.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/16.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/17.PNG?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m5/task5.3/screenshots/18.PNG?raw=true">
