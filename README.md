<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This project involves setting up and configuring osTicket to function efficiently as a ticketing system. The process includes creating multiple agents and assigning them to specific departments, defining roles, and setting appropriate permissions. Additionally, it covers configuring Service Level Agreements (SLAs), organizing help topics, and managing user accounts.






<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket
<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Admin/Analyst Login Page

- Configure End Users osTicket URL

- Configure Roles and Permissions

- Set Up Departments and Teams

- Enable Ticket Creation

- Configure Agents and Users

- Set Up Service Level Agreements (SLA)

- Configure Help Topics for Ticket Creation

<h2>Configuration Steps</h2>

<p>With osTicket open navigate to the Admin Panel by clicking "Admin Panel" located in orange at the top right of the page:

</p>

![Screenshot_33](https://github.com/user-attachments/assets/8aaee958-fb51-493a-92fa-d971dd7426a6)

<p>To start configuring Roles Navigate to the "Agents" tab and click on "Roles" underneath the "Agents" tab. Enter a role name:

</p>

![Screenshot_35](https://github.com/user-attachments/assets/ef171bfe-673b-4612-91ad-47dca364ce0b)

<br />

<p>

  ![Screenshot_36](https://github.com/user-attachments/assets/36f349de-1040-43c4-84d4-7e972be5abaa)

</p>In the "Permissions" tab of this role, give this role all permissions in "Tickets", "Tasks", and "Knowledgebase". This will be our "Supreme Admin" Role:
<p>

</p>
<br />

<p>

  ![Screenshot_37](https://github.com/user-attachments/assets/074332f4-a49c-4b89-a53a-7560ac4c97ea)

To set up departments, while still in the "Agents" tab, click on "Departments" located just below the "Agents" tab. Name the department "Sysadmins" and create the Department:

</p>

![Screenshot_38](https://github.com/user-attachments/assets/e9f7e31a-a6d7-4d32-a279-13fa546975b7)

<p>Next, create a team by selecting the "Teams" tab, while still in the "Agents" tab. Then, name the team "Online Banking" and create team:

</p>

![Screenshot_39](https://github.com/user-attachments/assets/15672ee9-1201-4bf8-a1b2-69fc06627b6d)

<br />Now, to allow anyone to create tickets, go to the "Settings" Tab, and under "Authentication Settings" make sure that "Require registration and login to create tickets" is unchecked:


![Screenshot_40](https://github.com/user-attachments/assets/e2c3dc2a-85ef-416c-8845-97caf38dc76b)

To create agents (the help desk workers) navigate back to the "Agents" tab and select "Agents" and fill out the name, email, and username:
- Jane (Dept: SysAdmins)
- John (Dept: Support)


![Screenshot_41](https://github.com/user-attachments/assets/9f90b409-e527-420a-875e-56d863dd41af)

Next to the username click "Set Password" set the password. Uncheck the "Send the agent a password reset email" and "Require password change at next login" options:

![Screenshot_42](https://github.com/user-attachments/assets/d2bb1d8a-c39f-4f66-9b7a-9d97a725c3fc)

On the "Access" tab for this user select the "SysAdmin" department and the "Supreme Admin" role created earlier:

![Screenshot_43](https://github.com/user-attachments/assets/90201587-638a-4ce3-8dcf-84a630e9f21a)

Under the "Teams" tab select "Online Banking" for this agent:


![Screenshot_44](https://github.com/user-attachments/assets/d803dbd8-26c8-4c40-8002-b132349efe34)

Then create one more agent (John Doe) as done previously, the only difference is in the "Access" tab select "Support" for the department:

Next, to create a user (the customers) switch to the "Agent Panel" in orange in the top right> Users> Add User and put an email and name, then create. (I also made one more user with the same steps taken here): user: Karen / karen@gmail.com


![Screenshot_45](https://github.com/user-attachments/assets/6f227e76-4806-4858-ac59-0d6beac39f59)

Configuring an SLA plan navigate back to Admin Panel> Manage> SLA create three SLAs with different severities, grace periods, and schedules like so:


![Screenshot_46](https://github.com/user-attachments/assets/085e07cf-a056-4b53-9e68-6c0bc4e8c693)


![Screenshot_47](https://github.com/user-attachments/assets/195ec6f0-6731-4cdd-b07c-fc697f4ce94e)


![Screenshot_48](https://github.com/user-attachments/assets/181429ae-7004-4f5c-9861-16b0c38cd269)

Under the same "Manage" tab go to the "Help Topics" tab and create four help topics named, "Business Critical Outage", "Personal Computer Issues", "Equipment Request", and "Password Reset" all with the same settings:


![Screenshot_49](https://github.com/user-attachments/assets/c8379644-9a51-4b7f-a8ca-31a62ea1e36a)


osTicket Setup Complete!
We've successfully set up multiple agents along with their departments, roles, and permissions. As well as, configured SLAs (Service Level Agreements), help topics, and users! osTicket is now setup for the next project where I will create and work different tickets using multiple agents and users!
