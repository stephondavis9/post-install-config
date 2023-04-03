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

- Add new Roles, Departments, and Teams.
- Add new Agents (workers), and allow anyone to create tickets.
- Add new Users (customers).
- Configure SLA.
- Configure Help Topics.

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/aS3xhT1.png" height="70%" width="70%" alt=""/>
</p>
<p>
<img src="https://i.imgur.com/ZjikYax.png" height="70%" width="70%" alt=""/>
</p>
<p>
<img src="https://i.imgur.com/XKYg7YH.png" height="70%" width="70%" alt=""/>
</p>
<p>
1. Use this link(http://localhost/osTicket/scp/login.php) to log into osTicket. Create a "Supreme Admin" role. Click "Admin Panel" -> "Agents" -> "Roles". Next, click "Add New Role" and name the role "Supreme Admin". Click the "Permissions" tab and enable every permission, next add the role. Next, add a new department. Next to the "Roles" tab, click the "Departments" tab and click "Add new Department". Name the department "System Administrators", leave the settings default, and click create. Next, create a new team and name it "Level II Support, add yourself as a member to the team. To create a new team, click the "Teams" tab, on the left side of the "roles" tab.
</p>
<br />

<p>
<img src="https://i.imgur.com/xWnQ0LR.png" height="70%" width="70%" alt=""/>
</p>
<p>
<img src="https://i.imgur.com/gmjVt83.png" height="70%" width="70%" alt=""/>
</p>
<p>
<img src="https://i.imgur.com/G68H2Z5.png" height="70%" width="70%" alt=""/>
</p>
<p>
2. Add new Agents(workers). While in the Admin Panel, click the "Agents" tab -> "Add New". Give the agent a name, email, username, and password. Next, click the "Access" tab and assign them to the "System Administrators" department with the role of "Supreme Admin". Lastly, add them to the "Level II Support" team. Next, create another agent. Assign agent #2 to the "Support" department with the role of "View Only". Next, allow anyone to create a ticket. While in the Admin panel, click settings -> Users -> then under "Authentication Settings" make sure "Require registration and login to create tickets" is unchecked. 
</p>
<br />

<p>
<img src="https://i.imgur.com/2YD1TL2.png" height="70%" width="70%" alt=""/>
</p>
<p>
3. Add new Users(customers). Switch to the "Agent Panel" -> click the "Users" tab -> click "Add User". Give the user a name and an email. Repeat to add an additional user.
</p>
<br />

<p>
<img src="https://i.imgur.com/KkKH0VN.png" height="70%" width="70%" alt=""/>
</p>
<p>
4. Configure SLA. Go back to the "Admin Panel" -> click "Manage" -> click the "SLA" tab -> click "Add New SLA Plan". Name it "SEV-A", make the schedule "24/7", and make the grace period "1 hour". Add another plan, name it "SEV-B", make the schedule "24/7", and make the grace period "4 hours". Add one more plan, name it "SEV-C", make the schedule "Monday - Friday 8 am - 5 pm", and make the grace period "8 hours".
</p>
<br />

<p>
<img src="https://i.imgur.com/5t2CeyS.png" height="70%" width="70%" alt=""/>
</p>
<p>
5. Configure Help Topics. While in the "Admin Panel", click "Manage" -> "Help Topics" -> "Add New Help Topic". Name the topic "Business Critical Outage", and leave the parent topic as is. Repeat the steps and create more help topics named "Personal Computer Issues", "Equipment Request", and "Password Reset". The osTicket post-installation steps are now complete.
<br />
