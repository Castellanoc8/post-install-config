# post-install-config
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-installation configuration of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents (Workers)
- Configure Users (Customers)
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/hc9SMu6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/Ty6NuHP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/614wSnq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/pXblpSK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To start off this tutorial, I had to first configure the Roles on osTicket. I did that by going to the Admin Panel, clicking on the Agents tab, and then on the Roles tab. Once I was in the Roles section, I clicked the "Add New Role" tab and created the Supreme Admin Role while also assigning it permissions. The permissions I assigned to the new role will allow certain access on to it on osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/foLIDxG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/vgrd8wA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the next step, I configured the Departments by going to the Agents section and clicking on the Departments tab. Inside the Departments section, I created a "New Department" and named it System Administrators.
</p>
<br />

<p>
<img src="https://i.imgur.com/bGFNJtZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/zq6w2tA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The next step in the process is me configuring the teams in this example. I did that by first making sure I was still in the Admin Panel and going into the Agents section. Once inside the Agents section i clicked on the teams tab and created two new teams and named them Level I Support and Level II Support. The teams need to be created because they allow agents from different departments to be pulled and organized to be able to handle specific issues or help a user via Help Topic or Ticket Finder.
</p>
<br />

<p>
<img src="https://i.imgur.com/1hTqLpy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
As I continued on, I edited the settings to allow anyone to create new tickets. To allow this to happen I went inside the settings and had to click on users, and inside the users settings I was able to edit and allow anyone to create new tickets.
</p>
<br />

<p>
<img src="https://i.imgur.com/S0VXI9l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/s82HZI9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/fwMuKn9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/HNDq80E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Moving forward, I had to edit the settings for the Agents(Workers). The settings I changed will give agents access to the help desk to be able to respond and resolve the tickets assigned to them. In order to do this, I went to the agents section and clicked "Add New Agent". Here I created to sample agents named Jane Doe and John Doe. I also edited their Access, Permissions, and the Team they would be assigned to.
</p>
<br />

<p>
<img src="https://i.imgur.com/T3nDqoF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/7QhQiPV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This step involved me creating new sample Users(Customers). First, I had to leave the Admin Panel and switch over to the Agent Panel on osTicket. When I switched over I clicked on the Users tab and clicked on "Add User". Here I created two new sample users who would be the customers in this scenario and named them Kelly Kelly and Ken Ken to keep it simple.
</p>
<br />

<p>
<img src="https://i.imgur.com/bdN5XSH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/TTiSu3N.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Moving ahead in this example, here I created and configured the companies SLA's. SLA's will very from company and are created to provide a timeframe of when the help desk admin expects the tickets to be resolved/closed. The way I configured the SLA's was by going back into the Admin Panel and clicking on the manage section. Once this section loaded I clicked on the SLA tab and selected "New SLA". Here I created 3 new SLA plans based on severity of the problem. The SLA's I created were SEV-A(1 hour, 24/7), SEV-B(4 hours, 24/7), and lastly SEV-C(8 hours, Business Hours).
</p>
<br />

<p>
<img src="https://i.imgur.com/HHAQiTI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/uYIDnt3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/6ljDeJO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the final step of this example, I created 4 new Help Topics that would help streamline the end-users experience to make sure topics are properly assigned and receive a fast responce to each ticket created. The Help Topics also determine what Department the ticket is sent to, which agent will have access to the ticket, and what SLA is assigned to that specific ticket. In order for me to create these Help Topics, I had to go back to the Manage tab in the Admin Panel and click on Help Topics. In here I was able to create the 4 new Help Topics which I named "Business Critical Outage", "Personal Computer Issues", "Equipment Request", and the final one is "Password Reset". In my last picture you will be able to see the Help Topics I created along with the default Help Topics that had already created when downloading osTicket.
</p>
<br />
