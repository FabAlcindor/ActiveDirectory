# ActiveDirectory
Set up Active Directory and Add a User to the Domain Server.
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Set up two Virtual Machines. One will be set up to be a user, the second will be set up as the Domain controller.
- Step 2: Using the Domain Controller, download and install active directory prerequisite.
- Step 3: Add the user to the server.
- Step 4: Login to the server using the user account

<h2>Deployment and Configuration Steps</h2>

<p>
<img width="499" alt="Screenshot 2023-08-26 155046" src="https://github.com/FabAlcindor/ActiveDirectory/assets/142107701/dd3646a0-1209-4367-97a8-9dde6b488477">
</p>
<p>
First set up the two virtual machines. The computer can be set up with specfications fitting the needs of the client, while the server should at the least have the configuration seen above. Within the Azure virtual machine portal, change the ip configuration of the domain controller from dynamic to static. 
</p>
<img width="781" alt="Capture1" src="https://github.com/FabAlcindor/ActiveDirectory/assets/142107701/4f6df035-57e8-4af9-89e9-cf6affbf639d">
<br />
</p>
Within the domain controller, access the firewall and changce inbound rules to allow for certain ICMP traffic. This will help with bringing the user into the server.
<br />

<p>
<img width="589" alt="Capture2" src="https://github.com/FabAlcindor/ActiveDirectory/assets/142107701/acb9d0d5-57f8-4106-9ed5-579a7e25719d">
</p>
<p>
On the Server, open the sever manager application and click "Add roles and features", This is how we will install active directory. The configurations could be adjusted to the needs of the user, but for this tutorial default configurations will work fine for most of the set up. When the installation process finsihes, click the flag to begin the deployment process. When the deployment window comes up make sure to click "add a new forrest".
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

