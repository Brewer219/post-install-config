<img width="280" height="420" alt="osTicket Logo" src="https://github.com/user-attachments/assets/2d18c1e2-b896-49dc-ab3a-3382e1b7d7ea" />

<h1>osTicket Configurations</h1>
This project demonstrates the configuration of core administrative components within an osTicket help desk environment. Building on the initial installation, the project focuses on organizing staff access, ticket routing, and service management by configuring roles, departments, teams, agents, users, service level agreements (SLAs), and help topics. The lab highlights how osTicket uses these components together to control permissions, separate responsibilities, prioritize issues, and support structured ticket workflows in a real-world support environment.<br />


<!--
<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)
-->

<h3>Environments and Technologies Used</h3>
<p align="left">
<img src="https://skillicons.dev/icons?i=azure,windows" />&nbsp;&nbsp;<img width="85" height="67" alt="osTicket Logo" src="https://github.com/user-attachments/assets/f5671aaf-1ad2-4741-b35e-54e8ec9fab53" />

- Cloud Platform: Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop: Microsoft Remote Desktop 3389
- Help Desk Software: osTicket
- Operating System: Windows  10/11



<h4>High-Level Deployment and Configuration Steps</h4>


**Key Actions**
 1.Configure Roles: Control agent permissions and access levels.
 2. Create Departments: Organize ticket ownership and collaboration
 3. Configure Teams: Group staff members for specific functions.
 4. Add Agents and Users: Simulate a real support environment.
 5. Define Service Levels Agreements (SLAs): and help topics to prioritize and route tickets automatically
 6. Create Help Topics: Categorize incoming tickets.

> [!IMPORTANT]
> Each step includes written instructions followed by a corresponding screenshot.
<br>Expand the **See screenshots** section to view the images.


> [!NOTE] 
> This project builds upon a prior lab where the Azure environment, virtual machine, and osTicket were initially deployed.

**Admin/Analyst/Agent Login Page:**
http://localhost/osTicket/scp/login.php 

**End Users osTicket URL:**
http://localhost/osTicket 



<h5>CONFIGURE ROLES</h5>
Roles in osTicket group related permissions and are assigned to staff to control what actions.
1. Login: Access the Admin/Analyst/Agent page at [Admin Login]
2. Navigate to Roles: Click on the Admin link at the top right, then select the 'Agent' tab and choose 'Roles'
3. Add new Role: Click +Add New Role.
- Role Name: Click +Add New Role.
- Permissions: Mark all checkboxes in the 'Tickets', 'Tasks', and 'Knowledgebase' tabs.
4. Save Role: Click Add Role.
<img width="450" height="230" alt="Step 28 Admin Panel Under Roles, Add Naming Role" src="https://github.com/user-attachments/assets/e5736156-b2f2-4931-9c93-3b4ec19ef969" /><img width="441" height="222" alt="Step 21 Admin Panel, Roles, All Access,Ticket Tab" src="https://github.com/user-attachments/assets/0398e29d-e47e-4d75-b706-84565dc54a99" /><img width="431" height="177" alt="Step 23 Admin Panel, Roles, All Access, click Knowledgeable Tab" src="https://github.com/user-attachments/assets/a6fa5e5a-ec88-4376-8d03-06652edda155" />





<h6>CONFIGURE DEPARTMENTS</h6>
<p>Departments seperate tickets to their assigned departments and ticket visibility, think Help Desk vs SysAdmins vs Networking.</p>
 1. Navigate to Departments: In the Admin Panel, select the department section under the Agents tab.
 2. Add New Department: Click +Add New Department.
   -Department Name: "SysAdmins"
 3. Access Settings: Click the Access tab to assign agents to the department if needed.
 4. Create Department: Click Create Dept.
<img width="345" height="440" alt="Step 34 Admin Panel, SysAdmins was created" src="https://github.com/user-attachments/assets/e3c2698f-cb60-4f33-ad8d-8f6e4ea0f072" />



<h7>CONFIGURE TEAMS</h7>
<p>Teams are used to group staff members from different departments who are responsible for a specific function.
1. Navigate to Teams: Select Teams from the 'Agents' Tab.
2. Add New Team: Click +Add New Team.
      -Team Name: "online Banking"
3. Create Team: Click Create Team
 
 For example, in a banking environment, a team might be created for online banking support and include a system administrator, a network technician, and help desk staff working together to resolve related issues. 

Select Teams from the Agents tab, and select +Add New Team.  For the Name, type Online Banking. Observe the settings and see different options that can be set, along with ability to assign Agents. Select Create Team</p>

<img width="463" height="333" alt="Step 36 click on the Teams Tab, the click create New Team button" src="https://github.com/user-attachments/assets/25a5d1e3-7aad-4f81-bac2-0a9c7dd27a64" /><img width="385" height="382" alt="Step 37 Admin Panel, Teams Field typing Online Banking in Name Field" src="https://github.com/user-attachments/assets/11d9c525-c175-43ef-832c-a561ef94112c" /><img width="377" height="319" alt="Step 38 Admin Panel, Team Field click Create Team Button for Online Banking Team part2" src="https://github.com/user-attachments/assets/273b76e1-9a8d-4fa3-bdf5-8499a5dc5831" />





<h8>CONFIGURE AGENTS</h8>
<p>Agents are the support staff in osTicket who handle incoming tickets, communicate with users, and update ticket status based on their assigned roles, departments, and teams. We will create two users. In the Agents tab, select the Agents section, and select +Add New Agent. Create Susan Smith, use any email.</p>
1. Add New Agent: In the Agents tab, select +Add New Agent.
- Agent 1:
 - Name: Susan Smith
 - Email: (Any valid email)
 - Username: Susan
 - Password: Password2
 - Department: SysAdmin
 - Role: Super Admin
 - Team: Online Banking
- Agent 2:
  - Name: Sam Hancock
  - Username: Sam
  - Password: Password3
  - Department: Support
  - Role: View Only
2. Settings: In the Settings tab, ensure "Require registration and login to create tickets" is unchecked.

<img width="324" height="328" alt="Step 43 Admin Panel, click Agent tab for online banking click Add New Agent" src="https://github.com/user-attachments/assets/b371baac-1309-4d4b-9a4e-c4ec75abddbb" /><img width="387" height="303" alt="Step 44 Admin Panel, Creating an actual Admin Account" src="https://github.com/user-attachments/assets/dda5ace7-d255-4715-b100-a679465749ac" /><img width="338" height="326" alt="Step 45 Admin Panel, Admin Account click Set Password" src="https://github.com/user-attachments/assets/0336d298-8402-4a78-a525-6868243b1443" /><img width="324" height="349" alt="Step 46 Admin Panel, Admin New Agent,can set the password" src="https://github.com/user-attachments/assets/dbd12861-b62d-453b-8bd5-9c4c47c094f3" /><img width="350" height="304" alt="Step 47 Admin Panel, Click Access Tab, and click Select Depart Dropdown" src="https://github.com/user-attachments/assets/69a08cb6-0a1b-4337-ae6b-663dde36d26d" /><img width="304" height="316" alt="Step 48 Admin Panel, click Select Role Dropdown" src="https://github.com/user-attachments/assets/9b113946-3297-4949-bf08-93d3f4905f74" /><img width="399" height="321" alt="Step 49 Admin Panel, Agents Teams click Online Banking" src="https://github.com/user-attachments/assets/6b0b2548-4140-4e92-a8ec-329ca0b22aff" />




<img width="333" height="337" alt="Step 51 Admin Panel, Create Agent Level 1 Help Desk Support" src="https://github.com/user-attachments/assets/269a8a88-6ad0-4a63-9c03-0589e28b7b1f" /><img width="368" height="300" alt="Step 52 Admin Panel, Agent Level 1 Help Desk hit Seclecting A Role" src="https://github.com/user-attachments/assets/a55ab9f1-8383-4f7d-8eec-0becfa5bf31a" /><img width="473" height="300" alt="Step 53 Admin Panel, Help Desk Level 1 hit Select A Role, View only" src="https://github.com/user-attachments/assets/d830cc28-0969-4888-b5c3-1762ca2b3c5b" />
<img width="374" height="309" alt="Step 57 Admin Panel, SysAdmin under Agents,Account Tab Type password" src="https://github.com/user-attachments/assets/e872bca0-9935-4b09-844b-492f12cc22e9" /><img width="459" height="339" alt="Step 59 Admin Panel, Agents Tab click on Sam Help Desk" src="https://github.com/user-attachments/assets/e3669695-e2eb-4f21-b628-241f997625b2" />






<h9> CONFIGURE USERS</h9>
<p>To add end users, we need to switch to Agent Panel, select Users tab, select +Add User. Choose any email, for name enter Joann and select Add User. Remember the email as end users will use their email addresses to create tickets, which we'll do in the next lab.</p>
1. Navigate to Users: Select Users tab and click +Add User.
  - User Name: 'Joann'
  - Email: (Any valid email)
2. Save User: Click Add User.

<img width="396" height="331" alt="Step 63 Agent Panel, click Users, the clck Add New Users Button" src="https://github.com/user-attachments/assets/5600b6ab-f1e6-4706-bfc1-3783face07f9" />
<img width="305" height="383" alt="Step 64 Agent Panel, creating a New User" src="https://github.com/user-attachments/assets/d2491c85-0974-4fef-83b7-c5fc80e15577" /><img width="330" height="304" alt="Step 65 Agent Panel, to config SLA&#39;s click Admin Panel" src="https://github.com/user-attachments/assets/11640d3d-4738-4760-b8ef-bea980914bb7" />




<h10>CONFIGURE SERVICE LEVEL AGREEMENTS (SLA)</h10>
<p>An SLA defines the expected response and resolution time for tickets based on priority or issue type.</p>

Back to the Admin panel, select Manage tab, and select SLA section Select +Add New SLA Plan. Here we'll create three new SLA Plans. 
 - Sev-A (Grace period: 1 Hour, Schedule: 24/7)
 - Sev-B (Grace period: 4 Hour, Schedule: 24/7)
 - Sev-C (Grace period: 8 Hour, Schedule: Business Hours)

   <img width="329" height="373" alt="Step 68 Admin Panel,in SLA Tab, click Add New SLA button" src="https://github.com/user-attachments/assets/9d8d946e-88ee-46db-ae6b-ca5be4ab7cda" /><img width="390" height="384" alt="Step 69 Admin Panel, SLA Tab Fill out the Fields, and hit Add Plan button" src="https://github.com/user-attachments/assets/2bb8a387-1a2c-4178-9aca-58258716babf" />


 
 > [!NOTE]
 > With SLAs, we can prioritize tickets by severity and business impact.</p>


<h11> CONFIGURE HELP TOPICS</h11>
<p>Help Topics help categorize incoming tickets and automatically route them to the appropriate department, priority, or workflow. Can be used by end users or agents.</p>
1. Navigate To Help Topics: In the Admin panel, under Manage tab, select Help Topics section.
2. Add New Help Topics: Click +Add New Help Topics.
   *Common Topics:
     *Business Critical Outage - Parent Topic:
    Report a Problem
     *Personal Computer Issues - Parent Topic:
    Report A Problem
     *Equipment Request - Parent Topic:
    General Inquiry
       *Password Reset - Parent Topic: Report a 
    Problem
      *Other - Parent Topic: General Inquiry 
 3. Save Help Topics: Click Add for each topic
<img width="352" height="350" alt="Step 71 Admin Panel, click Add New Help Topics" src="https://github.com/user-attachments/assets/8fb928b0-d918-4cd2-83e7-721317a90326" /><img width="327" height="325" alt="Step 72 Admin Panel, Help Topics Info type Business Critical Outage, select Report A Problem" src="https://github.com/user-attachments/assets/d6c84f48-7a1e-4879-85d2-0f8716b6ea38" /><img width="306" height="399" alt="Step 73 Admin Panel, Help Topics Added Successfully" src="https://github.com/user-attachments/assets/f949caf7-64d7-4037-8c5e-90e9986dd88e" />















