<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1 Configure Roles
Admin Panel -> Agents -> Roles
Supreme Admin
Configure Departments
Admin Panel -> Agents -> Departments
System Administrators
Configure Teams
Admin Panel -> Agents -> Teams
Level I Support
Level II Support



- Item 2 Allow anyone to create tickets
Admin Panel -> Settings -> User Settings
Registration Required: Require registration and login to create tickets 
Configure Agents (workers)
Admin Panel -> Agents -> Add New Jane
John

- Item 3 Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
Ken

- Item 4 Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (1 hour, 24/7)
Sev-B (4 hours, 24/7)
Sev-C (8 hours, business hours)

- Item 5 Configure Help Topics
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset


<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/UCKNfWl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On this Screen

Within the Admin Panel, there is now a convenient link to access the Agent Panel, allowing for seamless navigation between the two roles. An admin is responsible for configuring the osTicketing system, defining roles, establishing service level agreements (SLAs), and performing general administrative duties. This role is to that of a system administrator (sysadmin) in real-world scenarios. On the other hand, the agent, or regular help desk personnel, is responsible for actively working on tickets, assisting users, and utilizing the platform for day-to-day tasks, without involvement in its initial setup.
</p>
<br />

<p>
<img src="https://i.imgur.com/tmQN6hG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/x2Cth4a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Departments

  Once the OsTicketing system has been setup you'll have two departments automactically created. Additional departs will need to be created as shown in the the second picture. When creating a new department it may be benefical to have a predetermined SLA already laid out so that you have an appropriate level for the new department(s).
</p>
<br />

<p>
<img src="https://i.imgur.com/o62Guxs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Agents
  

Agents are granted access to the help desk with the purpose of addressing and resolving support tickets. When enlisting an Agent to the help desk, it becomes essential to assign them to a Primary Department and designate a Primary Role for handling the Tickets/Tasks directed to that specific department. Furthermore, Agents can be provided Extended Access to other departments within the help desk, along with the option to assign distinct roles for each department. These configurations can be managed in the Access section of the Agent's Profile.

Teams


Teams offer the flexibility to draw upon and reassign Agents from various Departments, enabling the organization to address specific issues or assist particular users based on Help Topics or Ticket Filters. When Agents from different Departments are assigned to a Team, their actions within that Team will take precedence over the rules defined by their respective Department parameters.
</p>
<br />
