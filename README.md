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

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure User/Customer
- Configure SLA
- Configure Help Topics (For users who create tickets)

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/SiGC7gN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/glbu157.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
</p>
<br />

<p>
<img src="https://i.imgur.com/lqMuYlF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/Ull5VsR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Roles: Roles are the permissions granted to Agents per Department that they have access to. To configure the roles for the agents in the osTicket system, I made sure I was logged in as an Admin. 
I then went into The admin panel> clicked "Agent" tab> clicked "Roles". 
This page shows 4 different roles with a set of permissions that can be checked/unchecked in association with a Department they have access to. 
In this tutorial, I created an additional role named "Supreme Admin". I went into the permissions tab and checked all the boxes, giving this role full access.
 
</p>
<br />

<p>
<img src="https://i.imgur.com/TsUxlb5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DPbxpie.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/SfhC0ZQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Departments: Since tickets are routed through Departments in the help desk, there are many settings that can be set for each Department. To configure the Departments for the agents in the osTicket system I made sure I was logged in as an Admin. 
I then went into the admin panel> clicked "Agent" tab> clicked "Departments".  In this tutorial, I added a new department named “SysAdmins” under the parent “Top-Level” department.

</p>
<br />

<p>
<img src="https://i.imgur.com/h5rFhOG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/rkz8fkt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Teams: Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter. To configure the Teams in the osTicket system I made sure I was logged in as an Admin. 
I then went into the admin panel> clicked "Agent" tab> clicked "Teams". In this tutorial, I added a new Team named “Online Banking”
</p>
<br />

<p>
<img src="https://i.imgur.com/I5G9d1z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/ht00Mxz.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/SFrFNWh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/BqDb49B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 Configuring Agents: To configure the Agents in the osTicket system I made sure I was logged in as an Admin. 
I then went into the admin panel> clicked "Agent" tab> clicked  “Add New Agent". In this tutorial, I added 2 new Agents. The first agent was named Jane Adams. In the Access tab, I added this agent to department “ SysAdmins” (which was created in the 2 previous steps) and added her to the role “Supreme Admin” (which was created in the first step). On Tab “Teams” I assigned her the “Online Banking” Team (created in the previous step). The second agent was named John Smith. In the Access tab, I added this agent to department “ Support”  and added him  to the role “view only” (for limited access). 
</p>
<br />

<p>
<img src="https://i.imgur.com/HIf81Jd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/sN3IyaT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Users: To configure the Users in the osTicket system, I made sure I was logged in as an Admin. I then went to the Agent Panel> click “Users” Tab > click “Add User” In this tutorial, I created one User named Karen Ramos.
</p>
<br />

<p>
<img src="https://i.imgur.com/T7P0YuO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring SLA: SLAs will vary from company to company and are designed to provide a timeframe of when the help desk admin expects the tickets to be resolved/closed. To configure the SLA in the osTicket system I made sure I was logged in as an Admin. I then went into the admin panel>click “Manage” tab> click “SLA> click “Add New SLA Plan”” In this tutorial, I created 3 different SLAs. They are as follows: Sev-A (Grace Period: 1 hour, Schedule: 24/7) Sev-B (Grace Period: 4 hours, Schedule: 24/7) Sev-C (Grace Period: 8 hours, Business Hours)

</p>
<br />

<p>
<img src="https://i.imgur.com/0JZd443.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Help Topics: Help Topics help streamline the end user's experience to ensure topics are correctly assigned and receive a fast response to each ticket made. The Help Topics also determine what Department the ticket is sent to, which agent will have access to the ticket, and what SLA is assigned to that ticket. To configure the Help Topics in the osTicket system I made sure I was logged in as an Admin. 
I then went into the admin panel> click “Manage” tab> click “Help Topics” >click “Add New Help Topics” I created 4 help topics : Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset, Other. This final step concludes my tutorial. 
</p>
<br />
