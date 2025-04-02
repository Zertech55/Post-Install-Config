<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Configuration</h1>
This tutorial outlines the configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

<h2>Configuration Steps</h2>

1. Configure Roles, Departments, and Teams
2. Allow end users to create tickets
3. Configure Agents and Users 
4. Configure SLA
5. Configure Help Topics


</p>
<p>
1. Configure Roles, Departments, and Teams
</p>
<br />
<p>
<img src="https://github.com/user-attachments/assets/603222ba-cf89-4cee-922c-ff9931ffc24a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://github.com/user-attachments/assets/2db0e0c0-fa26-4b29-909a-861e560305b4" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure roles, departments, and teams in osTicket, start by setting up departments, which are the primary organizational units for categorizing and routing tickets. In the admin panel, create departments under Manage > Departments, naming them, setting their status (active or archived), and deciding if they’re public or private (private ones are hidden from clients). You can also assign a manager, set an SLA for response times, and define a schedule. 
  
  Next, create teams if you need agents from different departments to collaborate on specific issues—go to Manage > Teams, name the team (e.g., "Critical Response Team"), and add agents from your staff list, optionally assigning a team leader for alerts.
  
  Finally, define roles to control permissions—navigate to Manage > Roles, create roles like "Support Agent" or "Manager," and check permissions such as viewing, replying, or deleting tickets. Assign these roles to agents within their departments via Agents > Edit Agent > Access. This process—departments first, then teams, then roles—ensures a structured setup for efficient ticket management.
</p>
<br />

</p>
<p>
2. Allow end users to create tickets
</p>
<br />
<p>
<img src="https://github.com/user-attachments/assets/bde62226-1021-4eeb-b62f-e64c49019777" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In certain scenarios, particularly in employee-only environments, it may be necessary to restrict ticket creation to registered users only. This can be achieved by enabling the "Registration Required" option, which is located in the admin panel under Settings > Users. By default, osTicket permits any user to create tickets; however, activating this setting ensures that only registered users have the ability to submit new tickets. This configuration enhances security and manageability, making it particularly valuable in environments where access control is a priority.
<br />

</p>
<p>
3. Configure agents and users
</p>
<br />
<p>
<img src="https://github.com/user-attachments/assets/09466bc6-4e1f-421d-aad8-c8a672dfbc72" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring agents and users in osTicket is a straightforward process that ensures your help desk system operates efficiently and securely. Users, who submit tickets, can be added manually via the admin panel or allowed to register themselves, depending on your setup. To organize users effectively, especially in larger environments, you can assign them to organizations, which helps in managing ticket access and automating workflows. For agents, who handle the tickets, you’ll need to create accounts with specific roles and permissions. Start by adding agents through agents > add new agent, assigning them to appropriate departments ex "IT Support and teams" if cross-departmental collaboration is needed. Roles, such as "Support Agent" or "Manager", define their permissions (e.g., viewing, replying, or closing tickets) and can be set under Manage > Roles. Additionally, configure email notifications for both users and agents to keep them informed of ticket updates and changes. Regularly reviewing and updating these configurations ensures your osTicket system remains secure and efficient.
</p>
<br />

</p>
<p>
4. Configure SLA
</p>
<br />
<p>
<img src="https://github.com/user-attachments/assets/29bda1bc-65ce-4a0e-9785-c0101b76f376" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
As an admin on osTicket, configuring Service Level Agreements (SLAs) is a key task to ensure timely ticket handling and meet customer expectations. To get started, log into the admin panel and go to the "Manage" tab, then select "SLA Plans". This section allows you to create, edit, or delete SLA plans. To create a new SLA, give it a descriptive name, set the grace period (the time before a ticket is considered overdue), and choose a schedule that reflects your team’s working hours and holidays, as this impacts how the grace period is calculated. You can assign SLAs to tickets based on factors like department, help topic, or specific agents, providing flexibility for managing different ticket priorities. Additionally, SLAs can include severity levels to trigger notifications or actions when deadlines are at risk. Once you’ve configured the settings, don’t forget to save your changes to activate the SLA across the system. This process helps maintain efficient and reliable support operations.
</p>
<br />

</p>
<p>
5. Configure Help Topics
</p>
<br />
<p>
<img src="https://github.com/user-attachments/assets/6ea307d1-a4e6-42a8-8d53-0a39e91ba4c2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring help topics in osTicket is incredibly helpful because it organizes incoming support requests into specific categories, such as "Billing Issues" or "Technical Support," allowing tickets to be automatically routed to the right department or agent. This ensures that issues are handled by the most qualified staff, reducing response times and boosting efficiency, which ultimately improves customer satisfaction. To set them up, log into the osTicket admin panel and go to Manage > Help Topics. From there, you can create new topics by adding a name and description, assign them to appropriate departments for accurate routing, and even enable auto-responses to acknowledge tickets or provide initial guidance. For more detailed organization, you can nest help topics into a hierarchy, like "Technical Support > Hardware Issues." Proper configuration streamlines the entire ticket management process, making it easier to prioritize and resolve issues effectively.
</p>
<br />



