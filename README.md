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

DEVOPS LECTURE 11 (Advance Shell Script):<br></br>
We will write a custom shell script which will detect the node health of our virtual machine. <br></br>
Let suppose we will write a custom shell script and put it in a git repository and if some one come to us and said I have a problem with my machine so we just run the script in that machine and be able to know or detect the issue.<br></br>
CUSTOM SHELL SCRIPT:<br></br>
Always write a meta data before the start of the script like (author name, date when script is written, purpose of the script and its version)
After this write the script and let suppose we write three command nproc, free -g and df -h and when we execute the script, we saw the combine output but don’t know which output is of which command so we can use an echo statement which works like a print statement (means before every output we get a print statement like: number of processes blaa blaa and then its output). <br></br>
set -x<br></br>
This approach is good but not best because let suppose if we have a 1000-line long scripts and 100 commands so we have to write echo statement every time which creates issue so what we do instead of that? We simply write set -x at the start of every script (-x represents this script is in debug mode) and output is something like this: Before the execution or output of the command we saw the command written itself like nproc or df -h. And also, sometimes we don’t want our user to see what commands should we use so, in that scenario we simply comment set -x.<br></br>

Ps -ef<br></br>
This is used to print the number of processes in your machine. Let suppose you are using chrome which uses a process, you are using a youtube application which uses and process and some other system processes. So, you use the command ps -ef. You can simply use the ps but it doesnot give you all the processes but when you use ps -ef it gives you all the processes. Ps means processes and -ef means entire details of process in full format.
When you see all the processes running on your system by using ps -ef command. Now , your task is to not just find out the processes but also find out the process ids <br</br>
Q: Let suppose your manager comes to you and said abdullah, find out the processes that are running by amazon and just get me the process ids<br></br>
A: So, first you write ps -ef command to see the processes that are running by amazon but it is a very long list and there’s a chance that you might skip some process so what you use?<br></br>
Ps -ef | grep “file name”/”amazon” (only fetch the required thing out of long list)<br></br>
You use a ps -ef | grep “amazon” command which gives you all the processes that are run by amazon but your manager wants the process id of these processes. Q: So, why manager wants process ids. A: because if he wants to kill, trip or dump the process he wants the process id<br></br>
| (Pipe parameter)<br></br>
ps -ef is one command and grep “amazon” is another command and who is integrating these two commands. Answer is pipe. What pipe can do? It can send the output of the first command to the second command. <br></br>
Let suppose you create a file like vim test1.sh and in that file you write
echo 1<br></br>
echo 12<br></br>
echo 11 <br></br>
echo 55<br></br>
echo 99<br></br>
So, now you want to only print those numbers that contains 1, so what you can do? You simply write this command ./test1.sh | grep 1 <br></br>
And your output is 1 11 12<br></br>
INTERVIEW QUESTION:<br></br>
As we discuss, ps -ef | grep “amazon” in this ps -ef gives us an output and with the help of pipeline this out is used by grep command. In the same way we see about ./test.sh | grep 1. <br></br>
But when we see about this command date | echo “today is “. We expected our output something like this: today is: Thu 12-01-2025 but our actual output is:  today is.<br></br>
This is because date is a by default command and it sends its output to stdin not to echo,<br></br>
In any system there are two channels or two log flows one is stdin and other us stdout or stderr <br></br>

DEVOPS LECTURE 12 (Advance Shell Script):<br></br>
Q: We have a question from previous lecture that our manager wants us to give him a process id of amazon processes running in our machine. We will see all about how we get processes running in our machine through ps -ef and then bring only amazon processes using ps -ef | grep “amazon”. It gives us all the detail of amazon processes but our manager only wants the process id of amazon not all details so we use awk command for that.
Awk command <br></br>
It is a process of filtering out the things. There are other commands similar to awk as well like cut and trim but awk is a powerful command. When you write ps -ef | grep “amazon” it gives you a complete sentence/detail like this:<br></br>
root         983       1  0 07:47 ?        00:00:01 /snap/amazon-ssm-agent/9881/amazon-ssm-agent<br></br>
ubuntu      1602    1179  0 07:55 pts/0    00:00:00 grep --color=auto amazon<br></br>

but awk is process of filtering out things. In this root is a string 983 is a string and all others are string. So, we just simply write an awk command to fetch our desired thing.<br></br>
Ps -ef | grep “amazon” | awk -F “ ” ‘{print$2}’<br></br>
This represents column 2 from multiple rows<br></br>
Combination of grep and awk command <br></br>
Let suppose I create one file named test and inside that test file I write:<br></br>
My name is Abdullah <br></br>
My employee id is 11<br></br>
So, outside the file when I use grep command to get name: I have to write like this:<br></br>
Grep name test -> output is: My name is Abdullah <br></br>
Or if I write: grep Abdullah test -> output is: My name is Abdullah <br></br>
So, syntax of grep is: (grep, write desired thing which I want to fetch, followed by file name)<br></br>
 Awk command<br></br>
For awk command I just know about the correct columns number like in this case: My name is Abdullah, there are total 4 columns. So how I write awk command.<br></br>
grep name test (not cnfrm) | awk -F “ ” ‘{print $4} -> output is Abdullah<br></br>
While writing grep and awk, always ensure that you use the right column numbers<br></br>
grep name test (not cnfrm) | awk -F “ ” ‘{print $4}: What this command means? In this command first grep command searches for lines in the file test.sh that contain the word "name".<br></br>
awk -F" " tells awk to use spaces as column separators.<br></br>
{print $4} means print the 4th word from each line found by grep.<br></br>
IMP NOTE:  The command that we are learning separately will place in the script at one place
Like we learn about ps -ef or grep or awk we just place these commands in our script<br></br>

Set -e and Set -o commands<br></br>
When we use pipeline and ps -ef or grep or awk in our script then we have to add some other things in our script as well and that other things are set -e and set -o. What they do? Answer is as follow:<br></br>
Set -e exits the script when there is an error. Let suppose there’s an error on line 1 but rest of your script is correct so, when you don’t add set -e then what happened? Ans is  your script will run which is not a good practice. Why it is not a good practice? The reason is, if your task is to first create a user and then create a folder and then create a file in that folder but if your user creation script is wrong then what you can do with folder and file creation. So, when there’s a set -e in your script. It detects the error and stops executing the script.<br></br>
Now, comes to the set -o. It is used in pipefail. Set -e is good but unable to detect the errors in case of pipeline so we use set -o. Let suppose there’s a command: <br></br>SEDEWDWEFE | echo.  Set -e consider this command as a correct command because it only checks or the validate the last command after pipe, it don’t concern about the command before pipe so that’s why we used set -o instead set -e for pipeline.<br></br>
Set -o is also used to display shell option<br></br>
IMP NOTE: Instead of writing set -x, set -e, set -o in a separate line. There are some people who write all this in a one line and that command is : set -exo <br></br>



Curl Command<br></br>
Let suppose there are 100 machines or apps out of which 99 are running fine and there’s an issue in one machine/app so as a devops engineer what you do? You simply first check the log file to check about the errors but usually log files are too big so people usually stored them on github or google storage or on some amazon storge like s3. So, in order to access that log file we use the curl command. It works like the postman or alternate of POSTMAN (not cnfrm), API fetching (not cnfrm)<br></br>
Curl file url | grep ERROR. When we write this command we get all the errors from the logfile<br></br>
Using the curl command we can retrieve any information from any external devices or internet<br></br>
Get Request through curl command<br></br>
We can also do a get request through curl command:<br></br>
Curl -X GET api.foodpanda.com<br></br>
OUTPUT OF THE ABOVE COMMAND:<br></br>
<html><br></br>
<head><title>301 Moved Permanently</title></head><br></br>
<body><br></br>
<center><h1>301 Moved Permanently</h1></center><br></br>
<hr><center>cloudflare</center><br></br>
</body><br></br>
</html><br></br>

Curl vs wget command<br></br>
There’s another command similar to curl command but what’s the difference between curl command and wget command is like when you simply write curl file url | grep ERROR it displays all the errors on the terminal but what about with the wget command. It first downloads the file in your system when you write this command: wget fileurl and then after that what you can do you use cat command along with file name let suppose cat filename so, you get a display of all the logfile on your terminal and when you add grep command with logfile like this: cat filename | grep ERROR then you get only the errors from the log file.<br></br>
Q: So, when to use curl and when to use wget?<br></br>
A: When you want to store logfile in your system as well then use wget command otherwise use curl command.<br></br>

8TH February, 2025<br></br>

DEVOPS LECTURE 13 (Advance Shell Script):<br></br>

Find command, root and sudo<br></br>
Find command as its name suggests it finds the file in the machine. But for the file command we should come as a root user or just a normal user. Root user you can say that is some sort of a admin who have the most privileges. In order to be a root user you have to write the command sudo su -. Sudo means switch user do and su means switch user. 
When I write the command find / name filename. / means all files in the machine<br></br>
<br></br>

If else<br></br>
a=5<br></br>
b=10<br></br>
if[$a > $b]<br></br>
then<br></br>
	echo “a is greater”<br></br>
else<br></br>
	echo “b is greater”<br></br>
fi<br></br>
for loop<br></br>
for i in [1.100]; do echo “$1”;done<br></br>
for<br></br>
do<br></br>
	increment<br></br>
done<br></br>

trap command<br></br>
trap command is a complex command. We used this command rarely in our script. It is used to trap the signals. Let suppose in a terminal you use ctrl c command to stop the execution so your terminal gets a signal like you have to stop or kill the execution. Let suppose you want that your process should not be kill by someone by writing or clicking some command. It should be kill by itself when there’s any issue or authorize access so what you can do? You can use a trap command which trap the signal. The command is: trap echo”don’t access without the permission of user” SIGINT (It means signal interrupt) there are multiple trap commands approximately 200.  <br></br>

INTERVIEW QUESTIONS<br></br>
Grep -o “s” <<<”$x” | wc -l<br></br>
-o in grep means only “s” means (only grep s of word Singapore) which is stored in x. It gives us the out 1 and the command wc -l means to count the length of word count,<br></br>

Crontab<br></br>
It is a linux command its work is simple like an alarm. Let suppose you are a linux admin and your job is to check the node health and give a report at every 6pm so instead of logging in every day. You simply use the crontab command<br></br>
Q: How we can open in the read only mode?<br></br>
A: vim -r test.txt<br></br>

SoftLink vs HardLink<br></br>
Softlink is like you create a file and save it in memory<br></br>
Hardlink is like you frequently use a file like copy it and modify it etc. So, instead of writing the cp command every time you just create a hardlink to any of the file(mirror a specific file) So, it creates a hardlink to the original file like if the original files get deleted, the other file remains same. (not cnfrm)<br></br>

Like python 3-> python<br></br>
./python <br></br>
So, this python actually refers to python3 and when you use ./python it actually executes python3 so python has a soft link to python 3 or we can say that python is an alias of python3 in memory and when we delete python3 python also gets deleted so it is a soft link<br></br>

Q: is bash dynamically or statically typed?<br></br>
A: Modern day languages like golang are statically typed and python are dynamically typed:<br></br>
e.g:<br></br>
python:<br></br>
x=5<br></br>
x=”string”<br></br>
golang:<br></br>
var x string <br></br>
(so, if you put numbers in x then it gives an error like x is expecting a string) <br></br>

Traceroute is used for network troubleshooting utility<br></br>
Let suppose your network is slow so, you simply write this command:<br></br>
Traceroute google.com<br></br>
We are trying to reach the google.com and see about the number of hops between traceroute and google.com<br></br>
From my laptop it will reach to the router from there it will reach to ISP router and from there it will take multiple hops and reach google.com.<br></br>
So, this command in short tells us about the how many hops and how much time each hop take<br></br>


Q: How will you sort list of names in a file?<br></br>
A: sort command<br></br>

Q: How will you manage logs of a system that generate logfiles everyday?<br></br>
A: So, in that case we use Logrotate command to upload our files somewhere out of the disk (not cnfrm)
We give it a proper format like Logrotate(gzip,etc)<br></br>

11st February, 2025<br></br>

DEVOPS LECTURE 14 (Live AWS Project using SHELL SCRIPTING for DevOps):<br></br>
Q: Why organizations move towards cloud architecture?<br></br>
A: Reason for moving towards cloud architecture is:<br></br>
1.	Management/manageability<br></br>
2.	Cost<br></br>
Let suppose you are starting a startup so in order to have a server, you must have data centers, you have to do a patching for security reasons and you must dedicate a proper team to manage and maintain these servers. And if you don’t use the server for a certain period of time then still you have to pay for it because it is in your data center but for cloud services you only pay for that time when you use the services. So, instead of doing all this one can simply move towards cloud architecture
Let suppose there are 100 employees in your company and every employee has an access to aws or aws resources. So, now it’s aws admin or devops engineer responsibility to check that either employee are using or utilizing aws services efficiently or not. Let suppose there’s one employee name x who create 100 EC2 instances that are used by no one or create EBs volume that are used by none of the EC2 instance but aws charged you for this because aws said I create/give a volume and instance to you, now you use it or not its not my responsibility. Give me my money. So, as aws admin or devops engineer must have a proper method and mechanism to check all this like your employee doesn’t waste any resources. <br></br>

As a devops engineer, your primary responsibility is to maintain the cost effectiveness and for that purpose you have to track the resource usage (Tracking resource usage). There are multiple ways for tracking resource usage. We don’t say shell scripting is an optimal way to do that there are multiple other ways like lambda function, python (boto3) as well.<br></br>


Now, let suppose there’s an organization name example.com and this organization use the resources like EC2, S3, lambda and IAM and your job is to keep track of resource usage by providing a detail to your manager on 6pm every day. (This is just for understanding. Devops engineer usually don’t follow this approach to send to the manager. They usually send tracking report to the reporting dashboard with the help of script).
Now how you use scripts to keep record or track. So, you write a script in which you create a file and in that file all the details are present like: instance active time, inactive time etc<br></br>


CronJob<br></br>
There’s a one thing to notice is we say to provide a detail resource tracking report to manager at 6pm every day. So, one way is that we have to run the script everyday at 6pm but what happened if we are not present at that time? If we are not present, then we use the cronjob and integerate it with our script so report will automatically send to the manager without running the script at 6pm. The purpose of cronjob is just like a timmer or alarm(Let suppose I have a youtube page and I have to upload a video on it at 7 pm but I am busy at 7 pm so what I can do? I simply upload a video at 3pm and set a timmer of 7pm which tells youtube to publish this video at 7pm automatically). So, cronjob is exactly the same<br></br>

What we can do at the end of the day? We are simply write shellscript and integrate it with cronjob<br></br>

Pipe more (| more)<br></br>
Using pipe more we can easily read output in a better way<br></br>

Aws  s3 ls<br></br>
Aws ec2 describe-instances<br></br>
Aws lambda list-functions<br></br>
Aws iam list-users<br></br>

JQ and YQ commands<br></br>
There are two very important commands jq and yq means json parser and yml parser respectively. Why these commands used? Answer is when when I write the above script it gives me all the detail, or list all the instances, lambda functions, s3 buckets etc but we only want the instance id so what we can do we simple use jq command. Let suppose I want an instance id of all my ec2 instances and this instance id is in instance locator which is also in resource locator so, how I write the command? The command is as follow:
aws ec2 dessccribe-instances | jq ‘.ResourceLocator[] .InstanceLocator[] . instanceId’<br></br>
In this way I get the instance id  (And this resource locator and instance locator are hypothethical it may vary in other machines)<br></br>

Now I want to add this script in my cronjob but before that I have to add this in file. So, how I can do that? I simply use ‘>’<br></br>

Aws  s3 ls > resourceTracker(name of the file)<br></br>
aws ec2 describe-instances | jq ‘.ResourceLocator[] .InstanceLocator[] . instanceId’ >> resourceTracker :q!<br></br>
Aws lambda list-functions > resourceTracker<br></br>
Aws iam list-users > resourceTracker<br></br>

After this integerate this with crontab which is our homework<br></br>
Homework Solution: <br></br>
We can simply run the crontab configuration using config -e<br></br>
And then write: 0 20 * * * /path to your script.sh<br></br>
(0 20 * * * * means that report will send to manager or reporting dashboard at exactly 8pm)<br></br>
save and exit the crontab editor<br></br>

There are 5 stars in crontab with space seperattion * * * * * in these five stars first two represents hours and minute(first represents minutes and second represents hours) and the rest 3 represents day of month, month, day of week respectively<br></br>

17th February, 2025<br></br>

DEVOPS LECTURE 15 (Shell Scripting Project GitHub Integeration):<br></br>
Let suppose as a devops engineer you maintain a github repositiory and monitor this repo for all type of vulnerabilities Ci/CD etc. Now assume someone came and say abdullah I want to see the number of collaborators on this repo so what you can do you can go to settings and then click on collaborators and then share the screenshot with that person so as a devops engineer you maintain all these things.<br></br>
Now assume another case, let suppose a person is resigning from an organization so as a devops engineer what your job is to revoke all of its permissions in the repo and if someone have a read access and now want a write access in the repo so a as a devops engineer you can give access to him.<br></br>
So, in short devops engineer have a lot of work with github repo that he/she maintain. So, instead of doing all this stuff manually or with the help UI. What we can do? We simply write the shell scripts and what the shell scripts required? Shell scripts require a github integeration<br></br>

How does this github integeration work? <br></br>
On a broader level there are two ways to integerate or talk to any application:<br></br>
One is API and other is CLI. So, we can talk to the applications like Github, Jenkins or Kubernetes with the help API. Kuberenetes most of the time use KubeCLT which is an easy utility instead of Api. In the same way github also uses CLI but for github API is preferable because it is present for a long time and with the help of shell scripting we can easily talk with the Api of any application and get our required data. <br></br>

Let suppose you write a github.com on search bar and github page opens so it means you communicate with the application through User interface but you can also communicate with the application programmatically like you use curl command to fetch Api in shell scripting (curl -x url with http protocol) or request command in python or with postman (And you can communicate programmatically only when these applications expose their API’s). So, when you use scripts or postman to communicate or talk with application, then it means you communicate with application programmatically.<br></br>

Q: Is devops engineer write API’s? <br></br>
A: No, as a devops engineer you only use or consume the Api’s. example is BOTO3.<br></br>
In order to talk to aws, you simply use the aws CLI utility to talk to the aws. It is the CLI way of talking/interacting with aws.<br></br>

The other way is you write a python program/script that uses BOTO3 which further interact with aws. It is the API way of talking/interacting with aws.<br></br>

For every API, there’s an API reference documnetation<br></br>
In order to communicate via API, devops engineer must go through API reference because devops engineer know how to use curl or request command but he don’t know how a certain API is written by developer or what is the url of a certain API or how a certain info should be get through url/api so, for that purpose he must go through the API reference.<br></br>

Let suppose I want a pull request in my repo. It is very easy in UI like I simple click on pull request and see all the lists of pull request. But how I can do this with scripts for that what url or what api url should I target in my scripts so that I get a list pull requests of my repo? So, for that first I go to github api doc and then on pull where I get the url and then add in the script will give me the list of pull requests.<br></br>

As a devops engineer, you maintain multiple github repositiories, manage multiple teams and each team have their own github repo and you grant them a right/proper access like which person can read which repo and which person can write which repo etc and then you can do CI/CD blaaa etc… <br></br>

In today’s lecture we write a script that displays a list of people who have access to the repo. 
Let say, someone resign from the company and today is his last day so as a devops engineer you see a list of people and if that person is granted an access you just simply revoke that access. Now every time you don’t need to go to github repo and then click on settings and then go to colloborators list blaa blaaa..So, what you can do? You simply list people who have access to the repo and if that resigning person have access so simply with shell scripting or with UI you revoke its access. So, inshort we automate the process with the help of scripts<br></br>

Let suppose you go to git hub repo github.com/kuberbetes/kubernest this is the official kuberenetes source code repo and you cannot see the collaborators in it because you are not the owner of this repo but most of the time these open source repos contains a file name owners in which all the collaborators are mentioned but when you are working in an organization as a devops engineer then you have an access of the collaborators. You simply click on the setting and then on the collaborators list. But this is the very boring task like everytime you have to login to the github and then search for the repo and then go to the settings and then on the collaborators. So, in order to get rid of this boring task we simply write a script that will display the list of collaborators of a specific repo<br></br>

<br></br>
22nd February, 2025 <br></br>
Day 8 of devops zero to hero done but practice not done so after FYP presentation 1 must do the practice of day 8 <br></br>

24th February, 2025 <br></br>

DEVOPS LECTURE 16 (Git and GitHub): <br></br>
Before discussing about git and github, Lets first discuss about version control because for git and github the foundation is version control. Why it becomes so popular and what are the important things or problems that version control addresses. These two problems that version control addresses are as follow:<br></br>
1.	Sharing<br></br>
2.	Versioning<br></br>

Let suppose there are 2 developers dev1 and dev2 and both of them are in same team and working on the same application (let suppose they are building and calculator) now dev1 works on the addition functionality and dev2 works on subtraction functionality. But at the end of the day they have to build the calculator their code must be on in one centralized place so for that reason they share code with eachother but code can be share through mails, slack and other platforms as well so why there’s a need of version control. See, we take a very basic example of calculator but in organization developers are building a very large large and heavy applications have a multiple files and dependencies so sharing through email or slack creates a lot of problems so that’s why version control is needed.<br></br>


Author-Abdullah
