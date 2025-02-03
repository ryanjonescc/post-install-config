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
