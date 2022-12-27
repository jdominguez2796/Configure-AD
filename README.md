<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Overview of Topology</h2>

<p>
<img src="https://i.imgur.com/uqxmlCW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Install Active Directory on the Windows Server. This VM will act as the Domain Controller (DC-1).
- Step 2: Promote DC-1 to a Domain Controller and create a Domain.
- Step 3: Create OU's (Organizational Units) for admins and employees.
- Step 4: 
- Step 5: 
- Step 6: 

<h2>Deployment and Configuration Steps</h2>

Step 1
<p>
<img src="https://i.imgur.com/EhiwlWG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On DC-1, navigate to server manager. Select "Manage" on the top right and click "Add Roles and Features" on the dropdown. Continue with the defaults until reaching the Server Roles step. Make sure to check the "Active Directory Domain Services" role. From here select next with default options on the rest of the installation steps. Select install on the final step. Wait for the installation to finish.
</p>
<br />

Step 2
<p>
<img src="https://i.imgur.com/DZbawp4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In Server Manager, on the top right the flag will have a yellow triangle with an exclamation mark. Click it and select "Promote this server to a Domain Controller". An AD Domain configuration window will pop up. Select add a new forest and type the name of your domain. Select next and create a password for the "DSRM". Select next and install for the rest of the steps leaving the default options and information. After completion, the server will restart. The server is now a Domain Controller. When you log in next, you will need to use the FQDN to log in. For example mydomain.com\username.
</p>
<br />

Step 3
<p>
<img src="https://i.imgur.com/aUeWrYQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In Server Manager, on the top right, select tools and click "Active Directory Users and Computers" from the drop down. On "mydomain.com" right click and select new and then organizational unit. Do this twice to create the admins and employees objects.
</p>
<br />

Step 4
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

Step 5
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

Step 6
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
