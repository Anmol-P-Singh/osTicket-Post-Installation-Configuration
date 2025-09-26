<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket – Post-Install Configuration</h1>
<p>This guide will walk you through setting up osTicket after installation — from creating roles and departments to setting up agents, users, and SLAs.</p>

<h2>🛠️ Tools & Tech Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
</ul>

<h2>💻 Operating System</h2>
<ul>
  <li>Windows 10 (21H2)</li>
</ul>

<h2>✅ Configuration Goals</h2>
<ul>
  <li>Set up Roles</li>
  <li>Set up Departments</li>
  <li>Set up Teams</li>
  <li>Add Agents (help desk workers)</li>
  <li>Add End Users (customers)</li>
  <li>Configure SLAs (Service Level Agreements)</li>
  <li>Set up Help Topics</li>
</ul>

<h2 align="center">🔐 Configure Roles</h2>
<p><strong>Navigation:</strong> <code>Admin Panel > Agents > Roles</code></p>
<p>Roles define the permissions that agents have in the system. Let’s set those up first.</p>

<!-- Step 1: Go to Roles -->
<p><strong>Step 1:</strong> Go to <code>Admin Panel > Agents > Roles</code> and click on <strong>Add New Role</strong>.</p>
<img width="829" height="473" src="https://github.com/user-attachments/assets/1ba8bdea-2066-4cf1-b5a6-58c39010c646" alt="Go to Roles Section"/>

<!-- Step 2: Enter Role Details -->
<p><strong>Step 2:</strong> Give your role a name (e.g., Support Agent), and add a short description if needed.</p>
<img width="828" height="583" src="https://github.com/user-attachments/assets/b0b2772e-f457-4eb5-a99b-ef058687d792" alt="Enter Role Details"/>

<!-- Step 3: Set Permissions -->
<p><strong>Step 3:</strong> Choose what this role can do by selecting the appropriate permissions.</p>
<img width="829" height="464" src="https://github.com/user-attachments/assets/db0c2b59-7ba9-48dc-91cd-edc17c1c2098" alt="Role Permissions"/>

<!-- Step 4: Assign Departments -->
<p><strong>Step 4:</strong> Assign this role to specific departments or make it available globally.</p>
<img width="828" height="340" src="https://github.com/user-attachments/assets/a53874f3-fd6a-4fe2-8646-80b68185ce9d" alt="Assign Departments"/>

<!-- Step 5: Save the Role -->
<p><strong>Step 5:</strong> Once everything looks good, click <strong>Add Role</strong> to save.</p>
<img width="825" height="379" src="https://github.com/user-attachments/assets/376672b6-6a18-4842-a0dd-584d1ecb0e5d" alt="Save Role"/>

<h2 align="center">🏢 Configure Departments</h2>
<p><strong>Navigation:</strong> <code>Admin Panel > Agents > Departments</code></p>
<p>Departments help organize your agents into groups based on their roles or areas of expertise. For example, you might have a <strong>System Administrators</strong> department, a <strong>Customer Support</strong> department, and so on.</p>

<!-- Step 1: Navigate to Departments -->
<p><strong>Step 1:</strong> Go to <code>Admin Panel > Agents > Departments</code>.</p>
<img width="831" height="555" src="https://github.com/user-attachments/assets/46e421ac-0841-45c6-af64-c9aff42857ab" alt="Departments screen"/>

<!-- Step 2: Add New Department -->
<p><strong>Step 2:</strong> Click on <strong>Add New Department</strong>.</p>

<!-- Step 3: Enter Department Details -->
<p><strong>Step 3:</strong> Enter the department name (e.g., <em>System Administrators</em>), set a description if desired, and assign any relevant managers or teams.</p>

<!-- Step 4: Save Department -->
<p><strong>Step 4:</strong> Click <strong>Add Department</strong> to save your new department.</p>

<p>Repeat these steps for each department you want to create. Properly setting up departments helps route tickets to the right groups and manage permissions effectively.</p>


<h2 align="center">👥 Configure Teams</h2>
<p><strong>Navigation:</strong> <code>Admin Panel > Agents > Teams</code></p>
<p>Teams group agents working on similar issues or projects, making ticket routing and collaboration easier. For example, you could have an <strong>Online Banking Team</strong> or a <strong>Network Support Team</strong>.</p>

<!-- Step 1: Navigate to Teams -->
<p><strong>Step 1:</strong> Go to <code>Admin Panel > Agents > Teams</code>.</p>
<img width="957" height="673" src="https://github.com/user-attachments/assets/c94f56f3-839d-48e2-a95c-01f39473858c" alt="Teams screen"/>

<!-- Step 2: Add New Team -->
<p><strong>Step 2:</strong> Click on <strong>Add New Team</strong>.</p>

<!-- Step 3: Enter Team Details -->
<p><strong>Step 3:</strong> Enter the team name (e.g., <em>Online Banking Team</em>) and add a description if needed.</p>

<!-- Step 4: Assign Agents -->
<p><strong>Step 4:</strong> Assign agents to the team to streamline ticket assignment and communication.</p>

<!-- Step 5: Save Team -->
<p><strong>Step 5:</strong> Click <strong>Add Team</strong> to save your new team.</p>

<p>Setting up teams helps your help desk work more efficiently by grouping agents based on their specialties or projects.</p>


<!-- Allow Anyone to Create a Ticket -->
<h2 align="center">✉️ Let Anyone Submit a Ticket</h2>
<p><strong>Navigation:</strong> <code>Admin Panel > Settings > User Settings</code></p>
<p>Make sure the option <em>"Require registration and login to create tickets"</em> is <strong>unchecked</strong>. This allows anyone to create a ticket without logging in.</p>
<img width="828" height="561" src="https://github.com/user-attachments/assets/990558ed-a3f9-4040-8831-b478e7113aca" alt="Allow Guest Tickets"/>

<!-- Configure Agents -->
<h2 align="center">🧑‍💼 Add Agents (Help Desk Staff)</h2>
<p><strong>Navigation:</strong> <code>Admin Panel > Agents > Add New</code></p>
<p>Agents are your help desk staff who will manage and respond to tickets. Let’s add some agents to get your team ready.</p>

<!-- Step 1: Go to Add New Agent -->
<p><strong>Step 1:</strong> Navigate to <code>Admin Panel > Agents > Add New</code>.</p>
<img width="951" height="809" src="https://github.com/user-attachments/assets/524b0adf-9324-4611-8375-f8ef5a95fcc7" alt="Add New Agent"/>

<!-- Step 2: Fill in Agent Details -->
<p><strong>Step 2:</strong> Enter the agent’s details such as name, email, and username. For example:</p>
<ul>
  <li><strong>Ben Crawford</strong></li>
  <li><strong>Jane Doe</strong></li>
</ul>
<img width="952" height="813" src="https://github.com/user-attachments/assets/fa90c704-ff38-4f65-ae63-a8218890e7b0" alt="Agent Details"/>

<!-- Step 3: Assign Departments -->
<p><strong>Step 3:</strong> Assign the agent to the appropriate department(s) so they can manage relevant tickets. For instance, assign to the <strong>Support</strong> department.</p>
<img width="957" height="397" src="https://github.com/user-attachments/assets/1b04352e-afed-45c1-a5ce-13d2e87ffda6" alt="Assign Agent Departments"/>

<!-- Step 4: Save Agent -->
<p><strong>Step 4:</strong> Click <strong>Add Agent</strong> to save.</p>

<p>Repeat this process to add all your help desk agents.</p>


<!-- Configure Users -->
<h2 align="center">🙋‍♂️ Add End Users (Customers)</h2>
<p><strong>Navigation:</strong> <code>Admin Panel > Users > Add New</code></p>
<p>End Users are the people submitting tickets—usually your customers or internal users. Let’s add a few users so they can start submitting requests.</p>

<!-- Step 1: Go to Add New User -->
<p><strong>Step 1:</strong> Navigate to <code>Admin Panel > Users > Add New</code>.</p>

<!-- Step 2: Enter User Details -->
<p><strong>Step 2:</strong> Fill in the user’s details. Example:</p>
<ul>
  <li><strong>Karen</strong> (an internal user who can submit tickets)</li>
</ul>
<img width="643" height="389" src="https://github.com/user-attachments/assets/867e6744-583e-473a-82c0-917d16f72623" alt="Add End User Karen"/>

<!-- Step 3: Save User -->
<p><strong>Step 3:</strong> Click <strong>Add User</strong> to save.</p>

<p>Repeat for any other internal or external users who will be submitting tickets.</p>

<h2 align="center">⏱️ Set Up SLAs (Service Level Agreements)</h2>

<p><strong>Navigation:</strong> <code>Admin Panel > Manage > SLA</code></p>

<p>SLAs define the response and resolution time for tickets based on severity. Setting these up ensures your team meets expectations for different types of requests.</p>

<p>Here’s how to configure SLA plans in osTicket:</p>

<!-- Step 1 -->
<p><strong>Step 1:</strong> Go to <code>Admin Panel > Manage > SLA</code> and click on <strong>Add New SLA Plan</strong>.</p>
<img width="828" height="535" alt="SLA Sev-A" src="https://github.com/user-attachments/assets/d94ce8f0-bf22-4228-ac13-d19de8970702" />

<!-- Step 2 -->
<p><strong>Step 2:</strong> Create a plan for high-severity issues. For example:</p>
<ul>
  <li><strong>Name:</strong> Sev-A</li>
  <li><strong>Grace Period:</strong> 1 hour</li>
  <li><strong>Schedule:</strong> 24/7</li>
</ul>
<p>Click <strong>Add Plan</strong> to save.</p>

<!-- Step 3 -->
<img width="829" height="541" alt="SLA Sev-B" src="https://github.com/user-attachments/assets/b942ca46-f0fd-40be-b604-6fd84b6ef577" />
<p><strong>Step 3:</strong> Repeat for medium-severity issues:</p>
<ul>
  <li><strong>Name:</strong> Sev-B</li>
  <li><strong>Grace Period:</strong> 4 hours</li>
  <li><strong>Schedule:</strong> 24/7</li>
</ul>

<!-- Step 4 -->
<img width="830" height="526" alt="SLA Sev-C" src="https://github.com/user-attachments/assets/758a1d52-4a0b-47a2-b941-1792d237f6ee" />
<p><strong>Step 4:</strong> Finally, configure a plan for low-priority issues:</p>
<ul>
  <li><strong>Name:</strong> Sev-C</li>
  <li><strong>Grace Period:</strong> 8 hours</li>
  <li><strong>Schedule:</strong> Business Hours</li>
</ul>

<p>Once all SLAs are added, you can assign them to Help Topics or ticket filters to automate service level tracking.</p>

<h2 align="center">📋 Create Help Topics</h2>

<p><strong>Navigation:</strong> <code>Admin Panel > Manage > Help Topics</code></p>

<p>Help Topics make it easier for users to categorize their issues when submitting a ticket. They also help route the ticket to the correct department or SLA automatically.</p>

<p>Let’s create a few commonly used Help Topics:</p>

<!-- Step 1 -->
<p><strong>Step 1:</strong> Go to <code>Admin Panel > Manage > Help Topics</code> and click <strong>Add New Help Topic</strong>.</p>
<img width="828" height="548" alt="Help Topic - Business Critical" src="https://github.com/user-attachments/assets/7d3e5f91-7e28-4ddf-838e-be2ec38328d9" />

<!-- Step 2 -->
<p><strong>Step 2:</strong> Fill in the topic name and details. Example:</p>
<ul>
  <li><strong>Topic:</strong> Business Critical Outage</li>
  <li><strong>Status:</strong> Active</li>
  <li><strong>Assign to Department:</strong> IT Support (or your relevant department)</li>
</ul>
<img width="827" height="549" alt="Help Topic - Personal Computer Issues" src="https://github.com/user-attachments/assets/37b05b06-e059-438c-82fd-878ab50b5967" />

<!-- Step 3 -->
<p><strong>Step 3:</strong> Repeat the process to add more Help Topics, such as:</p>
<ul>
  <li>Personal Computer Issues</li>
  <li>Equipment Request</li>
  <li>Password Reset</li>
</ul>

<img width="829" height="543" alt="Help Topic - Equipment Request" src="https://github.com/user-attachments/assets/72ae8c1d-43c8-4d0d-b892-227af6245087" />

<!-- Step 4 -->
<p><strong>Step 4:</strong> For each topic, double-check the following:</p>
<ul>
  <li>Correct department assignment</li>
  <li>Associated SLA (if needed)</li>
  <li>Ensure the topic is <strong>Active</strong> and visible to users</li>
</ul>

<img width="833" height="539" alt="Help Topic - Password Reset" src="https://github.com/user-attachments/assets/f67fd52c-b651-4524-a079-348f9dca46d6" />

<p>✅ Once completed, these topics will appear in the dropdown list when users submit a new ticket — making their requests easier to categorize and resolve efficiently.</p>

<!-- Wrap-up -->
<h2 align="center">🎉 Congratulations You're All Set!</h2>

