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


Author-Abdullah
