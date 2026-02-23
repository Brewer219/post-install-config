<img width="280" height="420" alt="osTicket Logo" src="https://github.com/user-attachments/assets/2d18c1e2-b896-49dc-ab3a-3382e1b7d7ea" />

<h1>osTicket Configurations</h1>
This project demonstrates the configuration of core administrative components within an osTicket help desk environment. Building on the initial installation, the project focuses on organizing staff access, ticket routing, and service management by configuring roles, departments, teams, agents, users, service level agreements (SLAs), and help topics. The lab highlights how osTicket uses these components together to control permissions, separate responsibilities, prioritize issues, and support structured ticket workflows in a real-world support environment.<br />




<h3>Environments and Technologies Used</h3>
<p align="left">


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


<img width="316" height="450" alt="Screenshot 2026-02-13 001923" src="https://github.com/user-attachments/assets/5fc7125f-e1ae-467b-b43d-00432c2b12d4" />


















**End Users osTicket URL:**
http://localhost/osTicket 


<img width="322" height="389" alt="Screenshot 2026-02-11 111058" src="https://github.com/user-attachments/assets/6d12fa4d-7c93-4638-ae0d-0dea39ff931a" />















<h5>CONFIGURE ROLES</h5>
Roles in osTicket group related permissions and are assigned to staff to control what actions.
1. Login: Access the Admin/Analyst/Agent page at [Admin Login]
2. Navigate to Roles: Click on the Admin link at the top right, then select the 'Agent' tab and choose 'Roles'
3. Add new Role: Click +Add New Role.
- Role Name: Click +Add New Role.
- Permissions: Mark all checkboxes in the 'Tickets', 'Tasks', and 'Knowledgebase' tabs.
4. Save Role: Click Add Role.






<h6>CONFIGURE DEPARTMENTS</h6>
<p>Departments seperate tickets to their assigned departments and ticket visibility, think Help Desk vs SysAdmins vs Networking.</p>
 1. Navigate to Departments: In the Admin Panel, select the department section under the Agents tab.
 2. Add New Department: Click +Add New Department.
   -Department Name: "SysAdmins"
 3. Access Settings: Click the Access tab to assign agents to the department if needed.
 4. Create Department: Click Create Dept.



<h7>CONFIGURE TEAMS</h7>
<p>Teams are used to group staff members from different departments who are responsible for a specific function.
1. Navigate to Teams: Select Teams from the 'Agents' Tab.
2. Add New Team: Click +Add New Team.
      -Team Name: "online Banking"
3. Create Team: Click Create Team
 
 For example, in a banking environment, a team might be created for online banking support and include a system administrator, a network technician, and help desk staff working together to resolve related issues. 

Select Teams from the Agents tab, and select +Add New Team.  For the Name, type Online Banking. Observe the settings and see different options that can be set, along with ability to assign Agents. Select Create Team</p>







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









<h9> CONFIGURE USERS</h9>
<p>To add end users, we need to switch to Agent Panel, select Users tab, select +Add User. Choose any email, for name enter Joann and select Add User. Remember the email as end users will use their email addresses to create tickets, which we'll do in the next lab.</p>
1. Navigate to Users: Select Users tab and click +Add User.
  - User Name: 'Joann'
  - Email: (Any valid email)
2. Save User: Click Add User.



<h10>CONFIGURE SERVICE LEVEL AGREEMENTS (SLA)</h10>
<p>An SLA defines the expected response and resolution time for tickets based on priority or issue type.</p>

Back to the Admin panel, select Manage tab, and select SLA section Select +Add New SLA Plan. Here we'll create three new SLA Plans. 
 - Sev-A (Grace period: 1 Hour, Schedule: 24/7)
 - Sev-B (Grace period: 4 Hour, Schedule: 24/7)
 - Sev-C (Grace period: 8 Hour, Schedule: Business Hours)

   

 
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
















