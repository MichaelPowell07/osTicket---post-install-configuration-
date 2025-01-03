p align="center">
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

- Ackowledge the difference between the Agent Panel and the Admin panel.
- Configure Roles to define permissions for agents.
- Set up Departments to group tickets by areas of responsibillity.
- Create teams to pull agents from multiple departments.
- Configure user settings to allow or restrict ticket creation.
- Add Agents (workers) and users (Customers).
- Set up Service Level Agreements (SLA) for ticket response times.
- Create Help Topics for users to categorize their tickets.
  

<h2>Configuration Steps</h2>

1.) Acknowledge Agent panel vs Admin Panel 
- The Agent panel is used by agents to work on tickets.
- The Admin panel is used to manage system settings, configurations, and permissions.

2.) Configure Roles
- Navigate to Admin panel -> Agents -> Roles.
- Add a new role called Supreme Admin.
- Define permissions for agents based on the role they will have. In this lab, we will give permissions for rthe Tickets, Task, and Knowledgebase section.

![image](https://github.com/user-attachments/assets/0834b1d6-1dff-4122-ba41-d083a0dd73ca)

![image](https://github.com/user-attachments/assets/c4d0cc8e-ee65-46c7-b343-0f41851c1381)

3.) Configure Departments
- Navigate to Admin panel -> Agents -> Departments
- Add a new department called SysAdmins.
- Use departments to control ticket visibility and assign areas of responsibility (e.g., Help Desk, SysAdmins, Networking).
  
![image](https://github.com/user-attachments/assets/28e3e79b-de20-414c-a4a1-98dc0e2cb69e)


In the "Parent" section choose Top level Department.

4.) Configure Teams 
- Navigate to Admin panel -> Agents -> Teams.
- Create a new team called Online Banking.
- Pull agents from diffrent departments to form specialized teams.

  ![image](https://github.com/user-attachments/assets/e9d6812a-a119-4af8-8a8b-eca0001c7ffe)

  5.) Allow Anyone to Create Tickets
  - Navigate to Admin panel -> Settings -> User settings.
  - Uncheck Require registration and login to create tickets to enforce ticket creation by anyone.
  - Enable Public - Anyone can register to disable requiring users to register and login before creating tickets.
 
    ![image](https://github.com/user-attachments/assets/53648ad8-37d4-45f0-b51c-b0811ef696f0)

    6.) Configure Agents (Workers)
    - Navigate to Admin panel -> Agents -> Add new.
    - Add agents with the follwoing details
    - Jane: Assigned to the SysAdmins department.
    - John: Assigned to the Support department

      ![image](https://github.com/user-attachments/assets/4aef37b8-d501-42b0-b63c-e949250f08a4)

      ![image](https://github.com/user-attachments/assets/245a4931-bdee-49d0-a8c7-8d2fc49e630d)

      ![image](https://github.com/user-attachments/assets/01e6eb7b-5d95-4a16-b95b-2f98c1f06bc6)

      ![image](https://github.com/user-attachments/assets/628573b5-0e89-4e34-b289-3a0ab8cd1ade)

7.) Configure Users (Customers)
- Navigate to Agent panel -> Users -> Add new.
- Add users with the following details
- Karen
- Ken

  ![image](https://github.com/user-attachments/assets/381592cd-dbf3-44a8-b96a-08bc09faa657)

  8.) Configure SLA (Service Level Agreement)
  - Navigate to Admin panel -> Manage -> SLA.
  - Add the following SLA'S
  - Sev-A: Grace period = 1 hour , schedule 24/7
  - Sev-B: Grace period = 4 hours, schedule 24/7
  - Sev-C: Grace period = 8 hours, schedule Business hours

    ![image](https://github.com/user-attachments/assets/b26db5c1-4b8a-4799-b305-0d49c0308b85)

    ![image](https://github.com/user-attachments/assets/e6e10ad8-4c15-4030-87eb-b27b4458d154)

![image](https://github.com/user-attachments/assets/470a52c8-5fbe-476d-a7a5-2ddc33e84ec0)

9.) Configure Help Topics 
- Navigate to Admin panel -> Manage -> Help Topics.
- Add the following help topics for users to select when creating a ticket.
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other

 ![image](https://github.com/user-attachments/assets/36c01131-149d-49ce-a910-0aacf802e862)
 
![image](https://github.com/user-attachments/assets/30e4b1f7-5148-4152-ad43-82f2d40715ed)

![image](https://github.com/user-attachments/assets/e0fc78b5-b2c5-4ce3-a395-96c1d4aac888)

![image](https://github.com/user-attachments/assets/e9cc2999-37c4-4c8a-8663-738bd12c9566)

![image](https://github.com/user-attachments/assets/38d99e86-b848-45ee-bdd4-1d7839f1fdf2)

Conclusion

By completing the post- installation configuration steps, you have successfully customized osTicket to suit your organization's requirements. You are now able to start using osTicket to manage and resolve customer issues effectivly.


