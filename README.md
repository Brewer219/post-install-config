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









## <h5>CONFIGURE ROLES</h5>
Roles in osTicket group related permissions and are assigned to staff to control what actions.
1. Login: Access the Admin/Analyst/Agent page at [Admin Login]
2. Navigate to Roles: Click on the Admin link at the top right, then select the 'Agent' tab and choose 'Roles'
3. Add new Role: Click +Add New Role.
- Role Name: Click +Add New Role.
- Permissions: Mark all checkboxes in the 'Tickets', 'Tasks', and 'Knowledgebase' tabs.
4. Save Role: Click Add Role.

<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Log into the Admin page with your personal account that you signed up with and click on "Admin Panel" as shown in image below:</p>

<img width="321" height="467" alt="osTicket click &#39;Admin Panel&#39;" src="https://github.com/user-attachments/assets/38f6d70b-5200-4f83-8af5-cec474a71715" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once on "Admin Panel" where it says 'Agents Settings' page then place mouse on the 'Agents' tab and click the 'Roles' option as shown in the image 2 below:</p>

<img width="321" height="467" alt="Click the Right &#39;Agents&#39; tab and click &#39;Roles&#39;" src="https://github.com/user-attachments/assets/7e258a9f-2478-45af-aa93-54ccff93849b" />

<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once on 'Roles' page then click the "Add New Role" button shown in the image below:</p>

<img width="321" height="467" alt="Once inside the &#39;Roles&#39; dashboard then click &#39;Add New Roles&#39;" src="https://github.com/user-attachments/assets/444ceee8-aa88-4fec-9ac9-beb105f5631a" />

<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From there you'll be on "Add New Role" and on the 'Definition' tab in the 'Name:' you will type 'Supreme Admin' and then from below click the yellow button 'Add Role' shown in the image below:</p>


<img width="321" height="467" alt="In &#39;Add New Role&#39; type &#39;Name&#39; and then below click &#39;Add Role&#39;" src="https://github.com/user-attachments/assets/6585b64b-43db-4f2b-9213-974ddf00f88b" />


<details><summary>See screenshot 5</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Click 'Permissions' tab and make sure 'Ticket' section has all the options checked in all the boxes as shown in the image below:</p>

<img width="321" height="467" alt="Click &#39;Tickets&#39; the Add Role" src="https://github.com/user-attachments/assets/d5d2090f-f16c-47d8-bef1-66e1b1925872" />

<details><summary>See screenshot 6</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From 'Ticket' tab click the 'Task' section and make sure all the boxes are checked as shown image below:</p>

<img width="354" height="475" alt="Supreme Admin Tasks in &#39;Permissions&#39; tab" src="https://github.com/user-attachments/assets/4a9e6c4e-f801-4506-b4ff-2abf734a519e" />

<details><summary>See screenshot 7</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From 'Task' sections go to the 'Knowledgebase' section and make sure that option box is checked as shown in image below:</p>

<img width="359" height="475" alt="Role Supreme Admin in the &#39;Kownledgeable&#39; inside &#39;Permissions&#39; tab" src="https://github.com/user-attachments/assets/35b3ce84-79f4-4361-8c6c-84795d59b09a" />




<h6>CONFIGURE DEPARTMENTS</h6>
<p>Departments seperate tickets to their assigned departments and ticket visibility, think Help Desk vs SysAdmins vs Networking.</p>
 1. Navigate to Departments: In the Admin Panel, select the department section under the Agents tab.
 2. Add New Department: Click +Add New Department.
   -Department Name: "SysAdmins"
 3. Access Settings: Click the Access tab to assign agents to the department if needed.
 4. Create Department: Click Create Dept.
 
<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>On your personal admin page click 'Admin Panel' to get to 'Departments' as shown in the image below:</p>

<img width="321" height="467" alt="Trying to Configure &#39;Departments&#39; dashboard go to &#39;Admin Panel&#39;" src="https://github.com/user-attachments/assets/a18baa48-d9b4-49a8-a37d-cb49f3dce383" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From there place mouse on the 'Agents' tab and down below click on the 'Departments' options as shown in the image below:</p>


<img width="321" height="467" alt="Once inside Admin Panel page then inside &#39;Agent&#39; click &#39;Department&#39;" src="https://github.com/user-attachments/assets/8aed5cf0-61e9-46b3-8a5d-e750787594cd" />


<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once you click 'Department' options you will get to the 'Departments' page and click "Add New Department" button on the center right shown in image below:</p>


<img width="321" height="467" alt="In &#39;Departments&#39; dashboard and click &#39;Add New Department&#39;" src="https://github.com/user-attachments/assets/0f7ed6e8-14bc-4c1c-8b9d-1772a181351e" />


<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From there you will be on the "Add New Departments" and in the dropdown option select 'Support' and 'Name:' type "SysAdmins" as shown in Image below:</p>


<img width="321" height="467" alt="Inside &#39;Add New Department&#39; page click dropdown &#39;Support&#39; option and then in name field type &#39;SysAdmin&#39;" src="https://github.com/user-attachments/assets/29209a2e-51df-4919-bf6e-728d6d32c6cb" />

<details><summary>See screenshot 5</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Scroll down and click the "Create Dept" button as shown in image below:</p>

<img width="321" height="467" alt="In &#39;Add New Departments&#39; and after selecting &#39;Level Support&#39; and typing &#39;SysAdmin&#39; and click &#39;Create Dept&#39;" src="https://github.com/user-attachments/assets/fa4a0fea-662d-410e-b577-21c9710407f8" />


<details><summary>See screenshot 6</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Now go back to theDepartments page and you will see that 2 departments are successfully created as shown in the image below:</p>

<img width="325" height="475" alt="Click the &#39;Departments&#39; and you can see 2 Departments are created successfully" src="https://github.com/user-attachments/assets/f7b22047-395b-4b90-81ad-db5ceee51c2a" />





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
</details><p>Click the "Admin Panel" and place mouse on the 'Agents' tab and click the 'Teams' option as shown in image below:</p>

<img width="321" height="467" alt="In Admin Panel click on the &#39;Agents&#39; tab and click on &#39;Teams&#39;" src="https://github.com/user-attachments/assets/840746a4-b571-4065-b643-2fcbb5f92065" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>After clicking the 'Teams' option then click "Add New Team" button as shown in the image below:</p>

<img width="321" height="467" alt="In Teams page to configure teams click on &#39;Add New Teams&#39;" src="https://github.com/user-attachments/assets/2d81b700-f0b0-4bc5-96f2-cc6eb439b53a" />

<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once clicking the "Add New Team" button you will land on a page called "Add New Team" page and in the field below where it says 'Name: Online Banking' and make sure the "Status: Active" and then down below click the yellow 'Create Team' button as shown in the image below:</p>


<img width="321" height="467" alt="Inside Add New Team click &#39;Online Banking&#39; and then click &#39;Create Team&#39;" src="https://github.com/user-attachments/assets/2573ab02-8ec7-4c13-8ee3-062536c1f6a2" />

<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p> Now get back to the 'Teams' page and seeing that the 'Online Banking' team was successfully created as shown in the image below:</p>


<img width="321" height="467" alt="Getting back to the Teams page and seeing that &#39;Online Banking&#39; was successfully created" src="https://github.com/user-attachments/assets/c084069b-06be-4275-8de9-9c303397ce36" />






## <h8>CONFIGURE AGENTS</h8>
<p>Agents are the support staff in osTicket who handle incoming tickets, communicate with users, and update ticket status based on their assigned roles, departments, and teams. We will create two users. In the Agents tab, select the Agents section, and select +Add New Agent. Create Susan Smith, use any email.</p>
1. Add New Agent: In the Agents tab, select +Add New Agent.
- Agent 1:
  - Name: Samuel Hancock
  - Email: Samuel@lognpacific.com
  - Username: samuel
  - Password: Password4
  - Department: Support
  - Role: View Only
- Agent 2:
 - Name: Susan Smith
 - Email: (Any valid email)
 - Username: susan
 - Password: Password3
 - Department: SysAdmin
 - Role: Super Admin
 - Team: Online Banking
  

2. Settings: In the Settings tab, ensure "Require registration and login to create tickets" is unchecked.

<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>On your personal admin page click "Admin Panel" as shown in the image below:</p>

<img width="325" height="475" alt="osTicket click &#39;Admin Panel&#39;" src="https://github.com/user-attachments/assets/33ea2fda-a194-4400-92a8-13481a1cfa5b" />


<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once on 'System Settings and Preference' page place mouse on the 'Agents' option as shown in the image below:</p>

<img width="325" height="473" alt="For me VB admin in creating Samuel click the &#39;Admin Panel&#39; and click the &#39;Agents&#39; link" src="https://github.com/user-attachments/assets/936e63fc-a59a-4440-82e2-181e0a0f5e80" />

<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From there you will end up on the 'Agents' page and on the center right click "Add New Agent" button as shown in the image below:</p>

<img width="325" height="470" alt="On Agents Page click &#39;Add New Agent&#39;" src="https://github.com/user-attachments/assets/bdefc7c3-014b-4dea-bf16-b3b7ed682ec5" />

<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>After clicking the "Add New Agent" button then the 'Add New Agent' in the account tab will come up and what you do is type in the fields like "Samuel Hancock" in the "Name" field and in the "Email Address:' type "Samuel@lognpacific.com" and underneath the "Authentication" section for 'Username' field type 'samuel' as shown in the image below:</p>
<img width="325" height="474" alt="Inside the Add New Agent creating an account for Samuel and typing in all the fields" src="https://github.com/user-attachments/assets/b873ae0d-9a16-416e-a5e2-d9a748bb8570" />

<details><summary>See screenshot 5</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Then to set password click the 'Set Password' button as shown in the image below:</p>

<img width="325" height="470" alt="Inside of Samuel account to change password but click the &#39;Set Password&#39; button" src="https://github.com/user-attachments/assets/d91310be-d5df-4b7f-a861-a1b6d5422aa3" />

<details><summary>See screenshot 6</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Then in the "Set Agent Password" box it will pop-up for 'Samuel' account and in that box you will uncheck the box where it says"Send the agent password reset email" as  shown in my image below:</p>
<img width="325" height="470" alt="Once clicking &#39;Set Password&#39; button for setting Samuel password then click or uncheck that center box" src="https://github.com/user-attachments/assets/140e7852-ffd5-4e67-b28b-830720132338" />

<details><summary>See screenshot 7</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once the box is unchecked then you will have the option in the fields to type a new password and then confirm the new password and down below make sure "Require password change at next login" is unchecked box as shown in my image below:</p>

<img width="325" height="470" alt="For Samuel account when setting password make sure inside the &#39;Set Agent Password&#39; the second box is unchecked " src="https://github.com/user-attachments/assets/6a83ab04-e39d-499e-b869-f8ef68f7eb66" />

<details><summary>See screenshot 8</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once you type your password in the 'Set Agent Password' field then down below click the 'Set' button to have the password set on account now as shown in the image below:</p>
<img width="325" height="470" alt="Once I typed in new password for Samuel then click the &#39;Set&#39; button" src="https://github.com/user-attachments/assets/b1fd8ec9-fcf7-4ea9-8fdf-a52ef2d45771" />

<details><summary>See screenshot 9</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From there 'Add New Agent' on the page click the 'Access' tab and set 'Primary Department' section as 'Support' and second option dropdown as 'View only' and "Extended Access' section as 'Support' as shown in my image below:</p>

<img width="325" height="475" alt="Samuel in the &#39;View Only&#39; access Support tab" src="https://github.com/user-attachments/assets/42e57791-aee2-44fa-b1d3-094d111eca6f" />

<details><summary>See screenshot 10</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From there leave 'Access' tab and click the 'Permissions' tab and in the 'Users' section make sure all boxes are checked as shown in the image below:</p>

<img width="325" height="467" alt="Samuel account on &#39;Users&#39; and &#39;Permissions&#39; this what it look like" src="https://github.com/user-attachments/assets/d0fb4882-f87a-4629-95dd-fd6216c920b3" />


<details><summary>See screenshot 11</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Leave 'Users' section then go to the 'Organizations' section and have or make sure all boxes are checked box as shwon in the image below:</p>

<img width="325" height="470" alt="Samuel &#39;Organization&#39; category " src="https://github.com/user-attachments/assets/575f6e0f-e7e3-44a5-8032-b2d4a259f4b3" />

<details><summary>See screenshot 12</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Then leave the 'Organizations' tab and go to the 'Knowledgebase' tab and make sure that 'FAQ' box is checked as shown in the image below:</p>
<img width="325" height="470" alt="Samuel account and &#39;Knowledageble&#39; tab" src="https://github.com/user-attachments/assets/288865e1-2f57-471b-9517-ac8826c840a7" />

<details><summary>See screenshot 13</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Then go to 'Miscellaneous' tab and makes sure the boxes are only checked is 'Agent' and 'Department' box as shown in the image below:</p>

<img width="325" height="467" alt="Samuel miscellaneous tab in his account" src="https://github.com/user-attachments/assets/9aa23e20-a572-4269-897d-b6635badfd79" />

<details><summary>See screenshot 14</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Now below click the yellow 'Create' button and Samuel as 'Support Level 1' agent is successfully created as shown in the image below:</p>

<img width="330" height="475" alt="Samuel as &#39;Support Level 1&#39; is successfully created" src="https://github.com/user-attachments/assets/fd6a1b74-9514-4261-b378-62ec10d4e647" />

<details><summary>See screenshot 15</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Back to the 'Agents' page you will see "Samuel Hancock" created as shown in the image below:</p>

<img width="330" height="475" alt="Now on Agents page &#39;Samuel Hancock&#39; is created" src="https://github.com/user-attachments/assets/058bfd28-150b-4e06-bd59-03271e255ac0" />

<details><summary>See screenshot 16</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>On that same page click "Agent New Agent" again to make a system Administrator named "Susan Smith" as shown in the image below:</p>

<img width="330" height="475" alt="Now after creating &#39;Samuel Hancock&#39; now lets create &#39;Susan Smith&#39; as SysAdmin" src="https://github.com/user-attachments/assets/5f9feeb8-a8b5-433a-b2b2-acb0f68f62dd" />

<details><summary>See screenshot 17</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Now after clicking that button you will then be on the 'Account' tab automatically and type in the fields "Susan Smith" and type in the "Email Address: and type "Susan@lognpacific.com" and then go down to the "Authentication" section and in the "username" field type 'susan' as shown in the image below:</p>

<img width="330" height="470" alt="Once click the &#39;Add New Agent&#39; button then type in &#39;Susan Smith&#39; in the field and type emails, and username" src="https://github.com/user-attachments/assets/b34533bf-d280-48d9-b349-5bb394d87eea" />

<details><summary>See screenshot 18</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>click on "Set Password" button as shown in the image below:</p>

<img width="335" height="473" alt="Now for &#39;Susan&#39; account click the &#39;Set Password&#39; button" src="https://github.com/user-attachments/assets/e96f7de7-9adb-4b2c-b9b0-184f1aa78fde" />

<details><summary>See screenshot 19</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once the box pop-up click or uncheck the box that says "Send the agent a password reset email" as shown in the image below:</p>

<img width="335" height="470" alt="Susan for the &#39;Set Agent Password&#39; unchecked the box" src="https://github.com/user-attachments/assets/f1bcd9b3-7612-4c41-b5fa-aa3ec049198e" />

<details><summary>See screenshot 20</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>The next thing you will do is type the new password and confirm password in the fields and make sure "Require password change at next login" is unchecked and then below click the "Set" button to set password on Susan's account as shown in the image below:</p>
<img width="335" height="470" alt="For Susan inside the &#39;Set Agent Password&#39; tpe in the fills and make sure the boxes are unchecked and then click &#39;Set&#39; button to set password" src="https://github.com/user-attachments/assets/a0b53252-a014-4b29-96e6-bd833271e4e2" />

<details><summary>See screenshot 21</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From there click on the 'Access' tab and under the "Primary Department" click the first dropdown and select 'Support/SysAdmins' and the second dropdown select "All Access" for Susan the SysAdmins and then lastly for "Extended Access" select "Support/SysAdmins" as shown in the image below:</p>

<img width="330" height="470" alt="Susan account susan has &#39;all access&#39; as SysAdmin" src="https://github.com/user-attachments/assets/8cf47060-17bc-4b8e-86e3-df226e1ea87f" />

<details><summary>See screenshot 22</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Now leave the 'Access' tab then go to 'Permissions' tab and click the 'Users' section and make sure all boxes are checked as shown in the image below:</p>

<img width="335" height="465" alt="Susans user link" src="https://github.com/user-attachments/assets/65e1e1b3-99eb-4331-a96b-b6786f0ff71b" />

<details><summary>See screenshot 23</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From the 'Users' section now leave and go to the 'Organizations' section and make sure all those boxes are checked as shown in the image below:</p>

<img width="330" height="465" alt="Susan organization in the &#39;Permissions&#39; tab" src="https://github.com/user-attachments/assets/e7b92485-7bcc-4c03-bbed-537d8d1bb3bb" />

<details><summary>See screenshot 24</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Now leave 'Organizations' and go to 'Knowledgebase' section and make sure "FAQ" is checked on Susan's account as shown in the image below:</p>

<img width="330" height="475" alt="Susans for permissions tab click &#39;Kownledageble&#39; link" src="https://github.com/user-attachments/assets/a036436e-231f-4de6-9589-383c782febef" />

<details><summary>See screenshot 25</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Once you leave 'Knowledgebase' then go to 'Miscellaneous' and make sure every box is checked on Susan's account as shown in the image below:</p>

<img width="330" height="470" alt="Susan account in permissions tab giving Miscullaneous giving all access with the checked boxes" src="https://github.com/user-attachments/assets/7aafbab0-f9eb-42fa-a96c-be4e2b071f76" />

<details><summary>See screenshot 26</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Now Leave the 'Permissions' tab entirely and cclick on the 'Teams" tab and once you're on the 'Teams' tab under the "Assigned Teams" tab click the dropdown box and select option called "new" option in the dropdown show in the image below:</p>

<img width="330" height="475" alt="Susan account in the &#39;Teams&#39; tab click the dropdown and click the &#39;Add New&#39; option" src="https://github.com/user-attachments/assets/f13a3aa3-d30b-4062-a068-8867d507a553" />

<details><summary>See screenshot 27</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>From there a "Add New Team" box will pop-up and the field you will put 'SysAdmin' and where it wants you to select a leader from a team just select "None" option as shown in the image below:</p>

<img width="335" height="470" alt="Make Susan Smith the &#39;SysAdmin&#39; and then click the &#39;Create&#39; button" src="https://github.com/user-attachments/assets/d1eddd90-6e73-4bdf-833c-ddfaf6c573b8" />

<details><summary>See screenshot 28</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Now "Susan Smith" is successfully added as SysAdmin by clicking the 'Create' button in yellow as shown in the image below:</p>

<img width="335" height="475" alt="For Susan account after clciking the yellow &#39;Create&#39; button below now Susan Smith is created as the &#39;SysAdmin" src="https://github.com/user-attachments/assets/a4ddff2c-dc70-45fb-a5c8-ed1bd4089e0e" />

<details><summary>See screenshot 29</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details><p>Then go back to the 'Agents' page and you will see 'Susan Smith' is successfully added as SysAdmin shown in the image below:</p>

<img width="335" height="470" alt="Now back to the Agents page or section both &#39;Samuel and Susan is now created in different departments&#39;" src="https://github.com/user-attachments/assets/c985cb56-f8ad-4484-bd38-334925a0af26" />





## <h9> CONFIGURE USERS</h9>
<p>To add end users, we need to switch to Agent Panel, select Users tab, select +Add User. Choose any email, for name enter Joann and select Add User. Remember the email as end users will use their email addresses to create tickets, which we'll do in the next lab.</p>
1. Navigate to Users: Select Users tab and click +Add User.
  - User Name: 'Joann'
  - Email: Joann@lognpacific.com
2. Save User: Click Add User.

<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
<img width="321" height="467" alt="Once in Agent Panel click on Users tab to create new users" src="https://github.com/user-attachments/assets/831d5471-1faf-4cff-9191-8144fb8bde22" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Once inside User Directory click the &#39;Add User&#39; button" src="https://github.com/user-attachments/assets/8c6474ae-54ff-40f8-87c9-a7de85e4f37d" />


<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Created a User name &#39;Joann&#39; (2)" src="https://github.com/user-attachments/assets/d0846889-c45c-4aef-99c7-933be82caa9b" />

<details><summary>See screenshot 5</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="321" height="467" alt="Joann the user is finally created" src="https://github.com/user-attachments/assets/6663dce5-a69c-4a0a-aec8-ead5995a53cf" />

<details><summary>See screenshot 6</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="332" height="465" alt="Once inside User Directory click the &#39;Add User&#39; button" src="https://github.com/user-attachments/assets/d93cd135-c24b-455c-9980-f7c0e9a11baf" />

<details><summary>See screenshot 7</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="343" height="460" alt="Creating user for Joesph" src="https://github.com/user-attachments/assets/c7021993-5825-4464-be0d-a45a241f3267" />

<details><summary>See screenshot 8</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="333" height="465" alt="Created Joesph account as a user" src="https://github.com/user-attachments/assets/618630f6-9083-4b2b-9648-6397519c2aab" />

<details><summary>See screenshot 9</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="350" height="478" alt="User Directory with All the Users Joesph and Joann" src="https://github.com/user-attachments/assets/d6c4ce71-24fc-4858-9825-8242aeaec637" />




## <h10>CONFIGURE SERVICE LEVEL AGREEMENTS (SLA)</h10>
<p>An SLA defines the expected response and resolution time for tickets based on priority or issue type.</p>

Back to the Admin panel, select Manage tab, and select SLA section Select +Add New SLA Plan. Here we'll create three new SLA Plans. 
 - Sev-A (Grace period: 1 Hour, Schedule: 24/7)
 - Sev-B (Grace period: 4 Hour, Schedule: 24/7)
 - Sev-C (Grace period: 8 Hour, Schedule: Business Hours)



<details><summary>See screenshot 1</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
<img width="356" height="470" alt="Going from Users page to Admin Panel click &#39;Manage&#39; tab" src="https://github.com/user-attachments/assets/63271760-287f-4e3b-ab04-c45bcc8abb4d" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="356" height="435" alt="Manage tab getting to the SLAs" src="https://github.com/user-attachments/assets/795791ad-e5ef-4a82-9959-200f7fe2de23" />

<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="356" height="467" alt="Once on SLA page the click &#39;Add New SLA Plan&#39; Button" src="https://github.com/user-attachments/assets/6cd16d69-90c3-4df9-8842-8f8dbf4d223d" />

<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="340" height="473" alt="Creating New SLA Sev A" src="https://github.com/user-attachments/assets/0661c956-6c44-4295-b75d-baeaa22689fd" />

<details><summary>See screenshot 5</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="356" height="475" alt="Adding New SLA Sev B" src="https://github.com/user-attachments/assets/7530b77b-3a1e-4535-b699-2de768455d6c" />

<details><summary>See screenshot 6</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="345" height="470" alt="Adding New SLA Sev C" src="https://github.com/user-attachments/assets/e287da04-081c-4c98-8253-51f9bb40a855" />

<details><summary>See screenshot 7</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="340" height="470" alt="All SLA are successfully created and Now go to &#39;Help Topics&#39;" src="https://github.com/user-attachments/assets/6b73a929-15be-45d5-8451-1e718717c385" />


 > [!NOTE]
 > With SLAs, we can prioritize tickets by severity and business impact.</p>


## <h11> CONFIGURE HELP TOPICS</h11>
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
 <img width="350" height="479" alt="How to going into Help Topics" src="https://github.com/user-attachments/assets/e84cff3f-d5bc-4128-a86a-77c034d0af8d" />

<details><summary>See screenshot 2</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="343" height="384" alt="Click &#39;Add New Help Topics&#39; again the 2nd time" src="https://github.com/user-attachments/assets/e5661210-5b69-4eb9-899e-bbb0f4a99cb5" />

<details><summary>See screenshot 3</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
<img width="354" height="473" alt="Then add the 2nd Help Topics &#39;Personal Computer Issues" src="https://github.com/user-attachments/assets/3c6d3ff4-a844-481c-a891-956da2c6daef" />

<details><summary>See screenshot 4</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
<img width="338" height="473" alt="Adding 3rd Help Topic Equipment Request" src="https://github.com/user-attachments/assets/0cfe29c9-9563-41fd-b708-0a141c77c4ef" />

<details><summary>See screenshot 5</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
<img width="351" height="473" alt="4th Help Topic Password Resets added" src="https://github.com/user-attachments/assets/beb0ffb5-3ac4-4388-8961-ae52ad51c9f9" />

<details><summary>See screenshot 6</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="369" height="419" alt="5th time &#39;Add New Help Topic&#39; on help topic page" src="https://github.com/user-attachments/assets/e0024119-d9fc-450a-b80a-c513a9e1fd4f" />

<details><summary>See screenshot 7</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
<img width="369" height="419" alt="5th time &#39;Add New Help Topic&#39; on help topic page" src="https://github.com/user-attachments/assets/a952416b-1795-4f08-b961-c9173c826200" />

<details><summary>See screenshot 8</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>
<img width="354" height="435" alt="5th Help Topic add &#39;Other&#39;" src="https://github.com/user-attachments/assets/63d562ab-c381-453c-a725-3f64f4204f4a" />


<details><summary>See screenshot 9</summary>
<img src="images/Step 3a.PNG" width="60%" >
</details>

<img width="349" height="476" alt="All Help Topics Fully Added" src="https://github.com/user-attachments/assets/cc14e187-57aa-4a20-b7a1-1dc28b2c95f7" />

















 


