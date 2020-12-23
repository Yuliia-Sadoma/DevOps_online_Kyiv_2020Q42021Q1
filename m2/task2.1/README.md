# Module 2 Virtualization and Cloud Basic

## Task 2.1

### PART 1. HYPERVISORS

#### 1. What are the most popular hypervisors for infrastructure virtualization?

* VMware vSphere
* Microsoft Hyper-V
* Azure Virtual Machines 
* Oracle VM

#### 2. Briefly describe the main differences of the most popular hypervisors.

There are two types of hypervisors:
* Type 1 Hypervisor (also called bare metal or native)
* Type 2 Hypervisor (also known as hosted hypervisors)

The main difference between Type 1 and Type 2 Hypervisor is that Type 1 Hypervisor runs directly on the host’s hardware while Type 2 Hypervisor runs on an operating system similar to other computer programs.

### PART 2. WORK WITH VIRTUALBOX

#### 1. First run VirtualBox and Virtual Machine (VM).

1.1-1.2 I got acquainted with the manual and downloaded VirtualBox for Windows and latest Ubuntu desctop.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen01.png?raw=true">

1.3 I created VM1 and installed Ubuntu.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen02.png?raw=true">

1.4 I got acquainted with the possibilities of VM1 control (start, stop, reboot, save state, etc.).

1.5 I created clone of existing VM1.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen03.png?raw=true">

1.6 VM1and VM2 was grouped.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen04.png?raw=true">

1.7 I tried to create a branched tree of snapshots, but I got such queue of snapshots.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen05.png?raw=true">

1.8 Export and import the VM1.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen07.png?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen08.png?raw=true">

#### 2. Configuration of virtual machines

2.1 VM configuration options was explored.

2.2 Configuring the USB.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen10.png?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen11.png?raw=true">

2.3 Configuring a shared folder.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen12.png?raw=true">

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen13.png?raw=true">

2.4 I configured different network modes for VM1, VM2, and made a table of possible connections.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen14.png?raw=true">

#### 3. Work with CLI through VBoxManage.

3.1-3.2 Executing the basic commands of VBoxManage list.

<img src="https://github.com/Yuliia-Sadoma/DevOps_online_Kyiv_2020Q42021Q1/blob/main/m2/task2.1/screenshots/screen15.png?raw=true">
