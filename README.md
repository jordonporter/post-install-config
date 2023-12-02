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

<h2>Tutorial Steps</h2>
<h3> Step 1: Configure Roles </h3> • First, we're going to create a special role called "Supreme Admin" that will have complete access to everything. To do this, head over to the Admin Panel. Click on "Agents," then go to "Roles," and choose "Add New Role." Now, give this role the name "Supreme Admin." 
</p>
• In the Permissions section, you'll see different areas where you can decide what this role can do. For the "Supreme Admin" role, we want them to have full access, so make sure to check every permission box. This will make this role capable of handling pretty much anything within the system.
</p>
<br />

![image](https://github.com/jordonporter/post-install-config/assets/144548453/755b1527-6174-43d3-8fc2-a7f96fd83ac3)
<br />
</p>

<h3> Step 2: Configure Departments </h3> • Next, we're going to make a new department in the Admin Panel. Here's how to do it: Go to "Agents," then "Departments," and click on "Add New Department." Name this department "System Administrators," and for this project, just keep all the default settings and click "Create Department."
</p>
<br />

![image](https://github.com/jordonporter/post-install-config/assets/144548453/5bee88a7-6f32-4002-987a-63c628a1358a)
</p>
<br />

<h3> Step 3: Configure Teams </h3> • Forming teams enables agents from diverse departments to work together collaboratively. To initiate the team creation process within the Admin Panel, start by going to "Agents," then "Teams," and finally, click on "Add New Team." Name this newly created team as "Level II Support." Afterward, move to the "Members" tab, where you can include yourself as a member of the team. This way, you can actively participate and cooperate within the "Level II Support" team.
</p>
<br />

![image](https://github.com/jordonporter/post-install-config/assets/144548453/939a2bad-3423-44c9-ae6d-6b265cd5536d)
</p>
<br />

<h3> Step 4: Allow Anyone To Create Tickets </h3> • To achieve this within the Admin Panel, navigate to "Settings," then "Users," then "Settings," and deselect the option for "Mandatory registration and login for ticket creation."
</p>
<br />

![image](https://github.com/jordonporter/post-install-config/assets/144548453/b2b45307-7eb4-48d8-8bd2-0550edfa5c6e)
</p>
<br />

<h3> Step 5: Configure Agents </h3> • Now, we'll create some agents. These are the folks who handle and solve customer issues. In the Admin Panel, find "Agents" and click "Add New Agent." Our first agent will be "Jane Doe" with the email "jane.doe@osticket.com" and username "jane.doe." Remember this username. Click "Set Password," uncheck "Send the agent a password reset email," and type in a password for Jane. Remember this password too. Uncheck "Require password change at next login" and click "Set."
</p>

• Now, you'll see different tabs. Here's where we can give Jane her permissions, assign her to a team, and specify her department. Under "Access," put Jane in the "System Administrators" department as a "Supreme Admin." In "Teams," add her to "Level II Support," and then click "Create."
a password for Jane. Remember this password too. Uncheck "Require password change at next login" and click "Set."
</p>

• Follow the same steps to make a second agent, "John Doe." Set his department as "Support" and "View only." Now, when you check "Agents," you'll see both Jane and John listed with their departments.
</p>
<br />

![image](https://github.com/jordonporter/post-install-config/assets/144548453/7f04b7d4-fee6-4003-b4c8-fd6943f0e1bb)
</p>
<br />
<h3> Step 6: Configure Users </h3> • Now, we'll set up the users, who are basically the folks who send in requests for help. To add a user, go to the "Agent Panel." Find "Users" and click "Create New User." Give the first user the name "Karen Karen" with the email "Karen@osticket.com," and then click "Add User." Now, let's add one more user, Ken. Just follow the same steps.
</p>
<br />

![image](https://github.com/jordonporter/post-install-config/assets/144548453/80d29cc5-5164-4f96-b2ea-c2c8f9bf4ec3)
</p>
<br />
<h3> Step 7: Configure SLAs </h3> • The purpose of the Service Level Agreement (SLA) is to prioritize requests and set a timeframe for resolving helpdesk tickets. Let's get started with this. Return to the "Admin Panel" and go to "Manage" and then "SLA" to create three SLA plans. Click "Add New SLA Plan" and name it "SEV A," with a grace period of "1" hour, and a schedule of "24/7." This means that any ticket that comes in should be resolved within 1 hour, no matter when it arrives.
</p>

• Now, create two more SLAs: one called "SEV B" with a grace period of "4" hours and a 24/7 schedule, and another named "SEV C" with an "8" hour grace period and a schedule from "Monday-Friday." This way, you've set up different response times for various types of requests.

</p>
<br />

![image](https://github.com/jordonporter/post-install-config/assets/144548453/26cce704-b863-4914-bdad-474a875c1158)
</p>
<br />
<h3> Step 8: Configure Help Topics </h3> • Setting up help topics makes it easier to organize user requests. In the Admin Panel, go to "Manage," then "Help Topics," and click on "Add New Help Topic." We're going to create four help topics: "Business Critical Outage," "Personal Computer Issues," "Equipment Request," and "Password Reset."
</p>
<br />

![image](https://github.com/jordonporter/post-install-config/assets/144548453/3762b013-9734-4d68-b741-3fda233d772d)
</p>
<p>
<br />
<br/>
<h2> That completes the post-install configuration of osTicket! </h2>

