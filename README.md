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


<h2>Configuration Steps</h2>

Now that osTicket was installed, it is time to setup admins, agents and roles. Click admin panel-> agents-> roles. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/4c4a5a5f-4d3f-42b9-8bea-67ffbc37aea1)

Adding a role "supreme admin". This role will have complete access and permissions. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/bfe0bf4b-a550-4704-b2fa-509e003c2131)

Configure Departments. admin panel-> agents-> departments. Now add a department named "system administrators". Each agent will belong to a department depending on their role at the helpdesk. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/4ee8f416-d685-47b5-a623-239cfd5d1812)

Configure a new team called Level II support. Admin Panel -> Agents -> Teams. Team will allow you to put together certain agenst for certain projects.

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/b618a67d-5281-4b3a-b6b4-9566b7e685c2)

Allow anyone to create tickets. Go to Admin Panel -> Settings -> User Settings. Registration Required: Require registration and login to create tickets. Enable this will allow anyone to create tickets so if any user is having a technical issue, they can create and submit a ticket so it can be resolved. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/6732ce77-a49b-4d48-87ae-129b52488ec4)

Next step is to create Agents. Agents are the helpdesk employees that resolve the technical issues whenever a helpdesk ticket is generated. They can be designated to a department (Level II support). Access, & Teams are be assigned in the Agents tab.

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/906d258c-ee18-4c3f-94d9-facbc2b40cc6)

Now to create the users. Users are the customers that submit the tickets to helpdesk. They don't work in the helpdesk department. To create a user follow this path Agent Panel->Users->User Directory->Add new.

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/f5a4fcaa-8347-4c37-a602-f60f3f62079b)

SLAs Plans provide a length of time in which the help desk is expected to take in order to solve a specific ticket. SLA Plans are created by going to Admin Panel->Manage->SLA Plans. Each SLA has a schedule and within that schedule there is a grace period. In this example SEV-A has a 24/7 and a one hour grace period.

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/37e0fcb6-6bf1-47ad-982d-0269c29563ed)


Configure help topics. These are topics that will be preset into the system for ease of reporting. Enter a topic name "Business Critical Outage" to describe the issue. Another one is personal computer issues. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/022695fa-9231-48a1-bed6-fbf1709e10f0)





