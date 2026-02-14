<img width="280" height="420" alt="osTicket Logo" src="https://github.com/user-attachments/assets/2d18c1e2-b896-49dc-ab3a-3382e1b7d7ea" />

<h1>osTicket Configurations</h1>
This project demonstrates the configuration of core administrative components within an osTicket help desk environment. Building on the initial installation, the project focuses on organizing staff access, ticket routing, and service management by configuring roles, departments, teams, agents, users, service level agreements (SLAs), and help topics. The lab highlights how osTicket uses these components together to control permissions, separate responsibilities, prioritize issues, and support structured ticket workflows in a real-world support environment.<br />


<!--
<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)
-->

<h2>Environments and Technologies Used</h2>
<p align="left">
<img src="https://skillicons.dev/icons?i=azure,windows" />&nbsp;&nbsp;<img width="85" height="67" alt="osTicket Logo" src="https://github.com/user-attachments/assets/f5671aaf-1ad2-4741-b35e-54e8ec9fab53" />

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10 (22H2)

<h2>High-Level Deployment and Configuration Steps</h2>


**Key Actions**
- Configure roles to control agent permissions and access levels
- Create departments and teams to organize ticket ownership and collaboration
- Add agents and end users to simulate a real support environment
- Define SLAs and help topics to prioritize and route tickets automatically

> [!IMPORTANT]
> Each step includes written instructions followed by a corresponding screenshot.
<br>Expand the **See screenshots** section to view the images.


> [!NOTE] 
> This project builds upon a prior lab where the Azure environment, virtual machine, and osTicket were initially deployed. <br />**[Part 1. osTicket: Prerequisites and Installation](https://github.com/MikeSays-1/osTicket-Install/)**

**Admin/Analyst/Agent Login Page:**
http://localhost/osTicket/scp/login.php 

**End Users osTicket URL:**
http://localhost/osTicket 

<h2>osTicket Configurations</h2> 

<h3>1. CONFIGURE ROLES</h3>
<p>Roles in osTicket group related permissions and are assigned to staff to control what actions they are allowed to perform, let's create a new role. Login to the Admin/Analyst/Agent page. You are currently viewing osTicket as an Agent, observe the Admin link in the top right and select it. From here, select the Agents tab, and select Roles. Select each role and observe each the Permission settings of each.

Select +Add New Role near the top-right of the Roles page. Name our Role "Super Admin", and in the Permissions tab, mark every checkbox in Tickets, Tasks, and Knowledgebase. Select Add Role.</p>
<img width="450" height="230" alt="Step 28 Admin Panel Under Roles, Add Naming Role" src="https://github.com/user-attachments/assets/e5736156-b2f2-4931-9c93-3b4ec19ef969" /><img width="441" height="222" alt="Step 21 Admin Panel, Roles, All Access,Ticket Tab" src="https://github.com/user-attachments/assets/0398e29d-e47e-4d75-b706-84565dc54a99" /><img width="431" height="177" alt="Step 23 Admin Panel, Roles, All Access, click Knowledgeable Tab" src="https://github.com/user-attachments/assets/a6fa5e5a-ec88-4376-8d03-06652edda155" />





<h3>2. CONFIGURE DEPARTMENTS</h3>
<p>Departments are used for seperating tickets to their assigned departments and ticket visibility, think Help Desk vs SysAdmins vs Networking. 

Let's create a new department. In Admin Panel, Agents tab, select the Departments section. Select +Add New Department. For the Name, type SysAdmins.  Observe the settings and see different options that can be set. Near the top, select the Access tab and observe that we are able to assign Agents to the department if needed. Select Create Dept. We'll assign agents to the department later.</p>
<img width="345" height="440" alt="Step 34 Admin Panel, SysAdmins was created" src="https://github.com/user-attachments/assets/e3c2698f-cb60-4f33-ad8d-8f6e4ea0f072" />



<h3>3. CONFIGURE TEAMS</h3>
<p>Teams are used to group staff members from different departments who are responsible for a specific function. For example, in a banking environment, a team might be created for online banking support and include a system administrator, a network technician, and help desk staff working together to resolve related issues. 

Select Teams from the Agents tab, and select +Add New Team.  For the Name, type Online Banking. Observe the settings and see different options that can be set, along with ability to assign Agents. Select Create Team</p>

<img width="463" height="333" alt="Step 36 click on the Teams Tab, the click create New Team button" src="https://github.com/user-attachments/assets/25a5d1e3-7aad-4f81-bac2-0a9c7dd27a64" /><img width="385" height="382" alt="Step 37 Admin Panel, Teams Field typing Online Banking in Name Field" src="https://github.com/user-attachments/assets/11d9c525-c175-43ef-832c-a561ef94112c" /><img width="377" height="319" alt="Step 38 Admin Panel, Team Field click Create Team Button for Online Banking Team part2" src="https://github.com/user-attachments/assets/273b76e1-9a8d-4fa3-bdf5-8499a5dc5831" />





<h3>4. CONFIGURE AGENTS</h3>
<p>Agents are the support staff in osTicket who handle incoming tickets, communicate with users, and update ticket status based on their assigned roles, departments, and teams.

We will create two users. In the Agents tab, select the Agents section, and select +Add New Agent. Create Susan Smith, use any email, set Username: Susan select Set Password. Unmark the Send the agent a password reset email, set password as <code>Password2</code>, unmark the Require password change at next logon checkbox and select Set. In Access tab, assign Susan to SysAdmin Department, Super Admins Role, and in Teams tab, assign to Online Banking Team and select Create. 

<img width="324" height="328" alt="Step 43 Admin Panel, click Agent tab for online banking click Add New Agent" src="https://github.com/user-attachments/assets/b371baac-1309-4d4b-9a4e-c4ec75abddbb" /><img width="387" height="303" alt="Step 44 Admin Panel, Creating an actual Admin Account" src="https://github.com/user-attachments/assets/dda5ace7-d255-4715-b100-a679465749ac" /><img width="338" height="326" alt="Step 45 Admin Panel, Admin Account click Set Password" src="https://github.com/user-attachments/assets/0336d298-8402-4a78-a525-6868243b1443" /><img width="324" height="349" alt="Step 46 Admin Panel, Admin New Agent,can set the password" src="https://github.com/user-attachments/assets/dbd12861-b62d-453b-8bd5-9c4c47c094f3" /><img width="350" height="304" alt="Step 47 Admin Panel, Click Access Tab, and click Select Depart Dropdown" src="https://github.com/user-attachments/assets/69a08cb6-0a1b-4337-ae6b-663dde36d26d" /><img width="304" height="316" alt="Step 48 Admin Panel, click Select Role Dropdown" src="https://github.com/user-attachments/assets/9b113946-3297-4949-bf08-93d3f4905f74" /><img width="399" height="321" alt="Step 49 Admin Panel, Agents Teams click Online Banking" src="https://github.com/user-attachments/assets/6b0b2548-4140-4e92-a8ec-329ca0b22aff" />








Create John Doe, username: john_user and set password to the same as Jane's for lab ease, and add user to Support Department, view only Role and select Create.

Before we leave the Admin panel, select the Settings tab, select Users section, and make sure we have the "Require registration and login to create tickets" checkbox unmarked.

<img width="333" height="337" alt="Step 51 Admin Panel, Create Agent Level 1 Help Desk Support" src="https://github.com/user-attachments/assets/269a8a88-6ad0-4a63-9c03-0589e28b7b1f" /><img width="368" height="300" alt="Step 52 Admin Panel, Agent Level 1 Help Desk hit Seclecting A Role" src="https://github.com/user-attachments/assets/a55ab9f1-8383-4f7d-8eec-0becfa5bf31a" /><img width="473" height="300" alt="Step 53 Admin Panel, Help Desk Level 1 hit Select A Role, View only" src="https://github.com/user-attachments/assets/d830cc28-0969-4888-b5c3-1762ca2b3c5b" />
<img width="374" height="309" alt="Step 57 Admin Panel, SysAdmin under Agents,Account Tab Type password" src="https://github.com/user-attachments/assets/e872bca0-9935-4b09-844b-492f12cc22e9" />





<h3>5. CONFIGURE USERS</h3>
<p>To add end users, we need to switch to Agent Panel, select Users tab, select +Add User. Choose any email, for name enter Karen and select Add User. Remember the email as end users will use their email addresses to create tickets, which we'll do in the next lab.</p>

<details><summary>See screenshots</summary>
<img src="images/Step 5a.PNG" width="40%" >
</details> 

<h3>6. CONFIGURE SERVICE LEVEL AGREEMENTS (SLA)</h3>
<p>An SLA defines the expected response and resolution time for tickets based on priority or issue type.

Back to the Admin panel, select Manage tab, and select SLA section Select +Add New SLA Plan. Here we'll create three new SLA Plans. 
 - Sev-A (Grace period: 1 Hour, Schedule: 24/7)
 - Sev-B (Grace period: 4 Hour, Schedule: 24/7)
 - Sev-C (Grace period: 8 Hour, Schedule: Business Hours)
 
 > [!NOTE]
 > With SLAs, we can prioritize tickets by severity and business impact.</p>

<details><summary>See screenshots</summary>
<img src="images/Step 6a.PNG" width="30%" > <img src="images/Step 6b.PNG" width="30%" > <img src="images/Step 6c.PNG" width="30%" >
</details> 

<h3>7. CONFIGURE HELP TOPICS</h3>
<p>Help Topics help categorize incoming tickets and automatically route them to the appropriate department, priority, or workflow. Can be used by end users or agents.

In Admin panel, under Manage tab, select Help Topics section. Select +Add New Help Topics. Create some common topics.
 - Business Critical Outage - Parent Topic: Report a Problem
 - Personal Computer Issues - Parent Topic: Report a Problem
 - Equipment Request        - Parent Topic: General Inquiry
 - Password Reset           - Parent Topic: Report a Problem
 - Other                    - Parent Topic: General Inquiry
 </p>

<details><summary>See screenshots</summary>
<img src="images/Step 7.PNG" width="40%" >
</details> 
