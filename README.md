<img width="280" height="420" alt="osTicket Logo" src="https://github.com/user-attachments/assets/2d18c1e2-b896-49dc-ab3a-3382e1b7d7ea" />

<h1>osTicket Configurations</h1>
<br>This project demonstrates the configuration of core administrative components within an osTicket help desk environment. Building on the initial installation, the project focuses on organizing staff access, ticket routing, and service management by configuring roles, departments, teams, agents, users, service level agreements (SLAs), and help topics. The lab highlights how osTicket uses these components together to control permissions, separate responsibilities, prioritize issues, and support structured ticket workflows in a real-world support environment.<br/>




<h3>Environments and Technologies Used</h3>
<p align="left">


- Cloud Platform: Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop: Microsoft Remote Desktop 3389
- Help Desk Software: osTicket
- Operating System: Windows  10/11



<h4>High-Level Deployment and Configuration Steps</h4>


**Key Actions**
 1. Configure Roles: Control agent permissions and access levels.
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


<details><summary>See screenshot</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

**Admin/Analyst/Agent Login Page:**
http://localhost/osTicket/scp/login.php 


<img width="316" height="450" alt="Screenshot 2026-02-13 001923" src="https://github.com/user-attachments/assets/5fc7125f-e1ae-467b-b43d-00432c2b12d4" />





**End Users osTicket URL:**
http://localhost/osTicket 

<details><summary>See screenshot</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>


<img width="322" height="389" alt="Screenshot 2026-02-11 111058" src="https://github.com/user-attachments/assets/6d12fa4d-7c93-4638-ae0d-0dea39ff931a" />















<h5>CONFIGURE ROLES</h5>
Roles in osTicket group related permissions and are assigned to staff to control what actions.
1. Login: Access the Admin/Analyst/Agent page at [Admin Login]
2. Navigate to Roles: Click on the Admin link at the top right, then select the 'Agent' tab and choose 'Roles'
3. Add new Role: Click +Add New Role.
- Role Name: Click +Add New Role.
- Permissions: Mark all checkboxes in the 'Tickets', 'Tasks', and 'Knowledgebase' tabs.
4. Save Role: Click Add Role.

<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="osTicket click &#39;Admin Panel&#39;" src="https://github.com/user-attachments/assets/38f6d70b-5200-4f83-8af5-cec474a71715" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Click the Right &#39;Agents&#39; tab and click &#39;Roles&#39;" src="https://github.com/user-attachments/assets/7e258a9f-2478-45af-aa93-54ccff93849b" />

<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Once inside the &#39;Roles&#39; dashboard then click &#39;Add New Roles&#39;" src="https://github.com/user-attachments/assets/444ceee8-aa88-4fec-9ac9-beb105f5631a" />

<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>


<img width="321" height="467" alt="In &#39;Add New Role&#39; type &#39;Name&#39; and then below click &#39;Add Role&#39;" src="https://github.com/user-attachments/assets/6585b64b-43db-4f2b-9213-974ddf00f88b" />


<details><summary>See screenshot 5</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Click &#39;Tickets&#39; the Add Role" src="https://github.com/user-attachments/assets/d5d2090f-f16c-47d8-bef1-66e1b1925872" />










<h6>CONFIGURE DEPARTMENTS</h6>
<p>Departments seperate tickets to their assigned departments and ticket visibility, think Help Desk vs SysAdmins vs Networking.</p>
 1. Navigate to Departments: In the Admin Panel, select the department section under the Agents tab.
 2. Add New Department: Click +Add New Department.
   -Department Name: "SysAdmins"
 3. Access Settings: Click the Access tab to assign agents to the department if needed.
 4. Create Department: Click Create Dept.
 
<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Trying to Configure &#39;Departments&#39; dashboard go to &#39;Admin Panel&#39;" src="https://github.com/user-attachments/assets/a18baa48-d9b4-49a8-a37d-cb49f3dce383" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>


<img width="321" height="467" alt="Once inside Admin Panel page then inside &#39;Agent&#39; click &#39;Department&#39;" src="https://github.com/user-attachments/assets/8aed5cf0-61e9-46b3-8a5d-e750787594cd" />


<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>


<img width="321" height="467" alt="In &#39;Departments&#39; dashboard and click &#39;Add New Department&#39;" src="https://github.com/user-attachments/assets/0f7ed6e8-14bc-4c1c-8b9d-1772a181351e" />


<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>


<img width="321" height="467" alt="Inside &#39;Add New Department&#39; page click dropdown &#39;Support&#39; option and then in name field type &#39;SysAdmin&#39;" src="https://github.com/user-attachments/assets/29209a2e-51df-4919-bf6e-728d6d32c6cb" />

<details><summary>See screenshot 5</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="In &#39;Add New Departments&#39; and after selecting &#39;Level Support&#39; and typing &#39;SysAdmin&#39; and click &#39;Create Dept&#39;" src="https://github.com/user-attachments/assets/fa4a0fea-662d-410e-b577-21c9710407f8" />

<details><summary>See screenshot 6</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Click the &#39;Create Depart&#39; for New Department page" src="https://github.com/user-attachments/assets/9e01f5a8-961c-4fab-9df9-7b1954736156" />

<details><summary>See screenshot 7</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Clicked on Agents tab Samuel from the Level 1 support depart is Created" src="https://github.com/user-attachments/assets/144f3e9d-0a7c-40a9-8d40-fcce72d567b9" />




### <h7>CONFIGURE TEAMS</h7>
Teams are used to group staff members from different departments who are responsible for a specific function.
1. Navigate to Teams: Select Teams from the 'Agents' Tab.
2. Add New Team: Click +Add New Team.
      -Team Name: "online Banking"
3. Create Team: Click Create Team
 
 <p>For example, in a banking environment, a team might be created for online banking support and include a system administrator, a network technician, and help desk staff working together to resolve related issues. 

Select Teams from the Agents tab, and select +Add New Team.  For the Name, type Online Banking. Observe the settings and see different options that can be set, along with ability to assign Agents. Select Create Team</p>

<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="In Admin Panel click on the &#39;Agents&#39; tab and click on &#39;Teams&#39;" src="https://github.com/user-attachments/assets/840746a4-b571-4065-b643-2fcbb5f92065" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="952" height="439" alt="In Teams page to configure teams click on &#39;Add New Teams&#39;" src="https://github.com/user-attachments/assets/2d81b700-f0b0-4bc5-96f2-cc6eb439b53a" />

<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>


<img width="321" height="467" alt="Inside Add New Team click &#39;Online Banking&#39; and then click &#39;Create Team&#39;" src="https://github.com/user-attachments/assets/2573ab02-8ec7-4c13-8ee3-062536c1f6a2" />

<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>


<img width="321" height="467" alt="Getting back to the Teams page and seeing that &#39;Online Banking&#39; was successfully created" src="https://github.com/user-attachments/assets/c084069b-06be-4275-8de9-9c303397ce36" />






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

<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>


<img width="333" height="337" alt="Step 51 Admin Panel, Create Agent Level 1 Help Desk Support" src="https://github.com/user-attachments/assets/5ada3f8e-422e-49ff-85ce-7b399c2abff1" /> 

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
<img width="313" height="331" alt="Step 58 Admin Panel, Accounts Tab click Agents" src="https://github.com/user-attachments/assets/386ca4fc-13dc-4f36-92e8-4c43e74118cf" />







<h9> CONFIGURE USERS</h9>
<p>To add end users, we need to switch to Agent Panel, select Users tab, select +Add User. Choose any email, for name enter Joann and select Add User. Remember the email as end users will use their email addresses to create tickets, which we'll do in the next lab.</p>
1. Navigate to Users: Select Users tab and click +Add User.
  - User Name: 'Joann'
  - Email: (Any valid email)
2. Save User: Click Add User.

<details><summary>See screenshot</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="396" height="431" alt="Step 63 Agent Panel, click Users, the clck Add New Users Button" src="https://github.com/user-attachments/assets/ef1328f1-0f95-4eb9-98b6-7eea6d05af37" />





<h10>CONFIGURE SERVICE LEVEL AGREEMENTS (SLA)</h10>
<p>An SLA defines the expected response and resolution time for tickets based on priority or issue type.</p>

Back to the Admin panel, select Manage tab, and select SLA section Select +Add New SLA Plan. Here we'll create three new SLA Plans. 
 - Sev-A (Grace period: 1 Hour, Schedule: 24/7)
 - Sev-B (Grace period: 4 Hour, Schedule: 24/7)
 - Sev-C (Grace period: 8 Hour, Schedule: Business Hours)

   <details><summary>See screenshot</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

   
<img width="390" height="384" alt="Step 69 Admin Panel, SLA Tab Fill out the Fields, and hit Add Plan button" src="https://github.com/user-attachments/assets/57b832f4-0111-4c36-b772-489d0a891ca0" />

   

 
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

<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
 

 <img width="352" height="350" alt="Step 71 Admin Panel, click Add New Help Topics" src="https://github.com/user-attachments/assets/78b78a13-2f78-44b4-b9d5-fa93c9e11eda" />

 <details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
 

<img width="306" height="399" alt="Step 73 Admin Panel, Help Topics Added Successfully" src="https://github.com/user-attachments/assets/7b85523d-956e-4d41-abf7-861077b64d25" />


















