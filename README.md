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

Now that osTicket is installed, it's time to setup admins, agents and roles. Click admin panel-> agents-> roles. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/7a840fb7-fe44-454d-95d8-0ce3e49acd85)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/e535af9f-c239-4c6d-8143-ab0175ca6268)



Adding a role "supreme admin". This role will have complete access and permissions. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/a3316c42-5bf5-4282-b0f0-0acc59cd9c23)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/35eb5afe-0fff-4f2c-affe-8713ca55a7ea)



Configure Departments. admin panel-> agents-> departments. Now add a department named "system administrators". Each agent will belong to a department depending on their role at the helpdesk. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/01ee806b-1b2f-46a9-9c71-675cf76c8147)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/90a5794a-ecc2-4d60-be4a-a49e52ab65ea)



Configure a new team called Level II support. Admin Panel -> Agents -> Teams. Team will allow you to put together certain agenst for certain projects.

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/c8fca03a-9aac-4b27-993d-516b1e112399)


Allow anyone to create tickets. Go to Admin Panel -> Settings -> User Settings. Make sure this is unchecked! Registration Required: Require registration and login to create tickets. Enabling this will allow anyone to create tickets so if any user is having a technical issue, they can create and submit a ticket so it can be resolved. Once it gets created, it will added to the queue then assigned to an agent by the queue manager. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/09b958ca-c772-4de2-a443-5d4877735ed3)



Next step is to create Agents. Agents are the helpdesk employees that resolve the technical issues whenever a helpdesk ticket is generated. Go to admin panel-> agents-> add new agent. We will name the agent John Doe and enter a username and email for this agent. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/d21baee7-afff-40e1-9621-c4697fe64327)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/42f16ec8-c6e1-40e6-95e5-1c263a985b05)



Now to create the users. Users are the customers that submit the tickets to helpdesk. They don't work in the helpdesk department. To create a user follow this path Agent Panel->Users->User Directory->Add new. We will name the user Steve. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/e36eea80-0b6d-438d-b7f3-54d62c221334)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/9ec4da1a-869e-40c8-9c23-0bf9ac645c29)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/8b095975-6e26-4791-a689-ae171029f016)






SLAs Plans provide a length of time in which the help desk is expected to take in order to solve a specific ticket. SLA Plans are created by going to Admin Panel->Manage->SLA Plans. Each SLA has a schedule and within that schedule there is a grace period. In this example SEV-A has a 24/7 and a one hour grace period. We can create the following SLA plans: Sev-A (1 hour, 24/7), Sev-B (4 hours, 24/7) and Sev-C (8 hours, business hours).


![image](https://github.com/AntIT-1/post-install-config/assets/141161539/03724ad0-ce83-4fee-803c-65b14a174a32)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/9c487b3c-b559-481e-b13e-ae9ac8e8f644)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/fc8368b4-e1c4-4b01-a38d-9f516c101d41)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/58b9c587-6e58-42e9-b3a8-7a859cad73cb)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/78fad4b3-99d0-43d7-bbb8-4cda7ab4a487)









Configure help topics. These are topics that will be preset into the system for ease of reporting. Enter a topic name "Business Critical Outage" to describe the issue. Another one is personal computer issues. 

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/5a82c0ff-c6bf-48c7-950e-cbdcd1f6a15b)

![image](https://github.com/AntIT-1/post-install-config/assets/141161539/a307b13f-180f-44ee-a2ef-befb1008fe51)







