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

Author-Abdullah
