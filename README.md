# Devops
<br></br>
20th January, 2025

<br></br>
DEVOPS LECTURE 1:

<br></br>
Q: What is Devops?

<br></br>
A: Basic Definition: 
Devops is a process/culture of improving the application delivery by ensuring proper automation, with a code/application quality that we maintained and also proper continuous monitoring and testing.

<br></br>
Q: Why Devops?

<br></br>
A: 10 years before, in order to deliver an app from your laptop/ from your end to customer end. Multiple entities are involved, 
First System Administrator who created a server and then there’s a tester who test the application on a server but before testing BRE deploy the application on the server and for deployment there must be a application server present on the server that holds the application and that Application server was created by server administrator after that Build and Release engineer put the application on a pre-production environment and then after successful testing BRE put the application/promoted the application to the production environment or on customer side. So, this complete process takes about 10 days. So, this is a time taking and manual process. So, to overcome or automate all these processes. The word Devops come into the picture.

<br></br>
Q: What are four pillars of Devops?

<br></br>
A: Four Pillars are as follow:
1. Automation
2. Quality
3.Monitoring
4. Testing
<br></br>
21st January, 2025
<br></br>
DEVOPS LECTURE 2:
<br></br>
SDLC:
<br></br>
We discussed phases of software development life cycle. Devops engineer comes mainly comes into picture at Building/development, testing and deployment phase. In development/building phase, the developer build the product and put its source code on some central point like Git and then QA team check this git code or test on virtual server and after successful testing this is put on the production environment means we deploy the product. So, the job of devops engineer is to automate all this process (building, testing, and deployment) and to make all this process fast/efficient.  Devops engineer itself don’t build, or test the product this is the job of a developer and tester respectively, Devops engineer just automate this process. 

22nd January, 2025
<br></br>
DEVOPS LECTURE 3:
<br></br>
VIRTUAL MACHINES:
<br></br>
Let suppose you own a 1-acre land and you build a house and a park and prayer area in it and you are living a happy life with your family in that 1 acre but still there is few space left in that area and when you give that space to someone for a rent then still you are living a happy life with your family in that area. So, you give your unused space/area for a rent and a person who buys that area on a rent can build their own house, park, prayer area etc on that rented area so now you are using your resources efficiently. Before giving area on rent you are wasting resources but now you are efficiently using resources and as a devops engineer our end goal is efficiency and automation 
<br></br>
SERVER AND VIRTUAL MACHINES:
<br></br>
Now we take a same example of rented area in that portion as well. Let suppose there’s an organization who owns 5 physical servers from HP/IBM. And this organization give 1 physical server to team 1, second physical server to team 2, third physical server to team 3 and so on. Now team 1 wants to deploy an app on server that uses only 5GB of the total server and 3 CPUs and the full capacity of server is let suppose 50GB and 10 CPUs so, the team waste the resources by using the server in that way. So, what we do? we install a hypervisor on the server which create a Virtual machine on a server. Hypervisor create a virtual machine on the same server of 50GB. Now on a 50GB server there are 5 virtual machines and each virtual machines have its own resources like they have their own CPU, memory etc and each team is using each Virtual machine. Instead of using 5 different physical servers now with the help of hypervisor 5 Virtual machines are created on a one/single server and 5 teams using each VM. Most common hypervisor are VM ware, XEN. This virtualization is not a physical separation of a server it is a virtualization/logical separation. In this way by doing virtualization, we add efficiency by using hypervisor.
<br></br>
HYPERVISOR
<br></br>
Hypervisor is a software, firmware or a hardware that allows one physical computer to run multiple virtual machines, each operating as if it were an independent machine.
<br></br>
23rd January, 2025
<br></br>
DEVOPS LECTURE 4:
<br></br>
Let suppose you have 100 requests to build a virtual machine so manually you have to login 100 times on aws or azure console and then make/request 100 virtual machines. But as a devops engineer our end goal is efficiency and automation so what we can do instead of logging in 100 times and manually make virtual machines what we can do? We write a scripts. The developer at amazon or devops engineer at amazon can expose an API and the user or devops engineer in an organization can write a script that request for aws API and in response they get a EC2 instance. (and the request must be valid, authenticated and authorized).
<br></br>
Q: When is terraform used?
<br></br>
A: the organization that used hybrid cloud pattern uses terraform (Hybrid cloud platform means some organization have their virtual machines in one cloud platform and other resources on other cloud platform).
<br></br>
24th January, 2025
<br></br>
DEVOPS LECTURE 5:
<br></br>
Make an account on aws and install a Mobatech
<br></br>
25th January, 2025
<br></br>
DEVOPS LECTURE 6:
<br></br>
Now first we will login to the virtual machine. First we do a login through aws console/UI. Now imagine you have 100 virtual machines. So, it’s a very difficult and boring task to login 100 times through aws UI/console (by going through aws console..click on login button etc blaa blaa) and also by logining in through aws you use aws terminal but people usually use/prefer fancy terminals like mobatech etc
<br></br>
AWS CLI:
<br></br>
It is an aws command line interface. Through this we can easily interact with aws services and create any resources on aws CLI and account.
<br></br>
26th January, 2025
<br></br>
DEVOPS LECTURE 7:
<br></br>
Operating System is a medium between software and hardware or it acts as a communication bridge between software and hardware.
<br></br>
As a user you’re installing an application on server then your server communicates with Operating System which further (operating system) communicate with the hardware like CPU etc  
<br></br>
Q: Why Linux is used among IT industry?
<br></br>
A: <br></br>
1.	Linux is free/open source<br></br>
2.	Linux is secure<br></br>
3.	You don’t have to install any kind of anti-viruses because most of the time Linux is secure<br></br>
4.	Linux have many distributions like ubuntu, redhat etc<br></br>
5.	The one thing that must have to be on your production system is speed (Like operating system must be fast. If operating system is slow then no matter how good you make an application or how modern technology you used, ultimately it causes many issues and problems). So, Linux is fast as compared to Windows<br></br>
<br></br>
VERY BASIC UNDERSTANDING OF LINUX ARCHITECTURE:<br></br>
Heart of Linux OS is kernel<br></br>
Compilers, User Processes, System Software
System Libraries
Kernel
<br></br>
The responsibility of kernel is to establish a communication between software and hardware.<br></br>
Primary responsibilities of kernel are as follow:<br></br>
1.	Device Management<br></br>
2.	Memory Management<br></br>
3.	Process Management<br></br>
4.	Handling System Related calls<br></br>
After kernal we have system libraries, System libraries are basically responsible for performing a task. Like user wants to do a certain task it first goes to system library and then to kernel<br></br>
FUNDAMENTALS OF SHELL SCRIPTING:<br></br>
Q: What is shell?<br></br>
A: Shell is a way that you talk to your OS.<br></br> 
Let suppose you want to create a file. So, it is very easy in Windows due to UI but let suppose you are working in a software house where there is not a proper UI for server or production environment so what you have to do now? You have to write commands to deal/communicate with server so somehow this type of thing is a shell scripting<br></br>
IMP NOTE: Linux is an operating system. Ubuntu, centos, fedora are Linux distributions<br></br>
Distributions are just vendors that provide Linux Operating System.
<br></br>
28th January, 2025
<br></br>
DEVOPS LECTURE 8:
<br></br>
Q: What is Bash?<br></br>
A:<br></br>
Bash (short for Bourne Again Shell) is a command-line interpreter or shell used in Unix-based operating systems like Linux and macOS. It is a powerful tool for interacting with the operating system, automating tasks, and managing system resources. Bash is both a command language for executing commands and a scripting language for writing scripts to automate repetitive tasks.<br></br>
Key Features of Bash:<br></br>
1.	Command Execution: Bash allows users to run commands to manage files, directories, processes, and more.<br></br>
2.	Scripting: It supports scripting for automating tasks, using loops, conditionals, and functions.<br></br>
3.	Built-in Tools: Includes utilities like grep, awk, sed, and others for text processing and task automation.<br></br>
4.	Environment Customization: Allows users to define variables, aliases, and functions to tailor their environment.<br></br>
5.	Job Control: Supports background processes and job control for multitasking.<br></br>
6.	Command History: Tracks commands you've run before, enabling you to re-execute them quickly.<br></br>
Common Use Cases:<br></br>
•	Automating repetitive system administration tasks (e.g., backups, updates).<br></br>
•	Writing shell scripts for DevOps pipelines.<br></br>
•	Running and managing server environments.<br></br>
•	Manipulating files and processing text data.<br></br>
•	Configuring software environments.<br></br>
Example Commands:<br></br>
•	ls: List files and directories.<br></br>
•	cd: Change the current directory.<br></br>
•	echo "Hello, World!": Print a message.<br></br>
•	grep "keyword" file.txt: Search for a keyword in a file.<br></br>
•	bash script.sh: Execute a Bash script.<br></br>
In summary, Bash is a fundamental tool for developers, sysadmins, and anyone working in Unix-like environments due to its versatility and simplicity.<br></br>

SHELL SCRIPTING:
<br></br>
For the memory, we use command free or free -g<br></br>
For CPU, we use the command nproc (Number of processing units)<br></br>
For disk, we use the command df -h (disk filesystem)<br></br>
For all things all at-once, we use the command top (table of processes)<br></br>
In case of ls -l or ls -ltr commands, we get a list like this -rwr—something like this so if this starts with dwr-rw—so in that case d means it is a directory.

<br></br>
30th January, 2025
<br></br>
DEVOPS LECTURE 9:<br></br>
Shell scripting is mainly used to automate the process<br></br>
Touch command is used for automation. Vi or vim command is used to create and opens/write the file at the same time but touch is used to only create the file.<br></br>
Q: Now question is why we use touch if vi or vim do the same work and have the more advantage than touch?<br></br>
A: Touch command is used for automation. Let suppose if someone comes and said Abullah make 100 files and if I use vim then it creates and opens the file at the same time so it makes an issue by opening all the 100 files at the same time which cause our machine to crash, that’s why we use touch command instead of vi or vim<br></br>
SHELL SCRIPTING:<br></br>
While writing the shell script the first command is shebang (#!) after shebang we write /bin/bash. 
Now understanding of the first line is very important. Some people use bash, some use ksh, some use sh and some use dash. Now question is what are the sh, ksh, bash, dash and many more? So, the answer is these are like the one who is responsible to execute our script like in case of java jdk is responsible for execution so these bash, sh and others are something like that.<br></br>
Q: Which one should we use?<br></br>
A: <br></br>
We use bash. They all are approximately similar with a little bit difference but it is very important to use the appropriate one. Now a days ksh is outdated most of the people uses bash and sh. And sh is indirectly a bash. Why I said this? Because when we use sh it makes a link with bash so that’s why I said that it is indirectly a bash. 
Let suppose you give a sh script to your colleague and on his machine same sh script doesnot run. Do you know why? The reason is from last year linux/ubuntu makes a linking with dash instead of bash so you don’t know that the sh on your friends/colleague machines link with what so that’s why there’s a chance of an error.
So, use of bash is preferable.<br></br>
EXECUTION:
<br></br>
Now in order to execute the script either you use ./file name or sh file name but when you hit enter it shows you “permission denied”. Either you make a file by yourself and write content by yourself but still linux ask you to first let me know who can execute this script or file because linux is very secure. So, in order to execute script or file you first have to set permissions <br></br>

CHMOD COMMAND:<br></br>
Chmod command basically changes the modification of the file. It has 3 categories like what permission a root user/administrator have, what permissions a group have and what permissions you have or anyone have? So, in order to give a permission there’s a magic number 7 which splits into formula 4,2,1. 4 means reads, 2 means write and 1 means execute. When I write this command on terminal (chmod 777 file name) it means to give all access to user, group and you or anyone (7 means full/all access: read, write and execute) and if you write this command: (chmod 444 file name ) now it means your user, group and you or anyone can only read the file and don’t write and execute the file.<br></br>

31st January, 2025
<br></br>
DEVOPS LECTURE 10 (Lec 9 Part 2):<br></br>
Famous commands:<br></br>
Touch-> to make file<br></br>
Cat -> If we don’t want to open the file just want to read the contents of the file then we use cat command<br></br>
Echo -> it is used to print text or variable on terminal<br></br>
Ls -> list all the files and folders in a directory <br></br>
Ls -l or ls -ltr -> to show detail listings with timestamp<br></br>
Pwd -> present working directory<br></br>
Cd -> change directory<br></br>
Vi or vim-> to create or write in a file using esc and I <br></br>
:wq!-> to write and save and then quit the file<br></br>
Man -> to show manual along with suffix<br></br>
Mkdir -> make directory along with suffix as a name<br></br>
Rm -rf -> remove directory along with suffix as a name<br></br>
Chmod->to change modifications of the file/grant permissions to the file<br></br>
History-> it shows you all the history like what command you used<br></br>
:q-> to simply quit the file without saving<br></br>
COMMENTS<br></br>
Comments are written by hashtag(#) in shell script<br></br>

HOW TO WRITE A SCRIPT<br></br>
First create and open a file using vim command and in that file write a script (As it’s my first script so I write a very easy and simple script : just make a directory name abd using mkdir command and then move to that directory using cd command and then create 2 files in abd using touch command) after that I save a file using :wq! Command and then set or grant permissions using chmod and then execute usin ./file name<br></br>
FIRST SCRIPT<br></br>
Vim sample-shell-script.sh<br></br>
INSIDE FILE / ACTUAL SCRIPT<br></br>
#!/bin/bash<br></br>
Mkdir abd<br></br>
Cd abd<br></br>
Touch file1.txt file2.txt<br></br>
OUTSIDE FILE / ACTUAL SCRIPT<br></br>
Chmod 777 sample-shell-script.sh<br></br>
./sample-shell-script.sh<br></br>

PURPOSE OF SHELL SCRIPTING IN DEVOPS<br></br>
Devops engineer can do many things like <br></br>
1.	infrastructure maintenance (to maintain the infrastructure of the organization)<br></br>
2.	code maintenance using git repositories (and most of the time they use linux because it is secure)<br></br>
3.	configuration management (there are also some tools available like ansible for this but still we write more scripts with more parameters according to our need).<br></br>

Let suppose there’s a guy name John working in amazon and the team in which they are working with using 1000 virtual machines (Linux). Now, developers’ complaint about node health or like their machine is working slowly. So, instead of checking the node health of all the 1000 machines manually what john do? He simply writes a script that automatically checks the machine and informed about the issue via email or some other resource. Now, John observes that this slow speed is due to memory shortage so he writes a custom script that automatically after two days check all the 1000 machines and informs John via email about performance like we found 10 suspicious machines from which 5 are due to memory and 5 are due to RAM. So, with the help of scripts the work of John become easier. <br></br>







Author-Abdullah
