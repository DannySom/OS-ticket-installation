<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Protocol (RDP) to securely connect to the virtual machine
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure subscription
- Windows 10 VM
- Ensure compatability with RDP using port 3389
- osTicket-Installation-Files.zip for setting up the installation

<h2>Installation Steps</h2>

<p>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/d70bbd2d-59d2-440d-9e24-3daf90a468b7" />

</p>
<p>
1. First, I created a virtual machine within Azure to host the osTicket help desk system.
</p>
<br />
</p>

<p>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/1a1d6dae-f586-4248-892b-4d9000b6daf7" />
___

</p>
<p>
2. Then, I downloaded the osTicket-Installation-Files.zip and unziped it onto my desktop within the virual machine. </p> This contains all the core application files needed to deploy osTicket.
  </p>
</p>
<br />

<p>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/a0310f41-84c0-4266-9ad8-b893708d4029" />

</p>
<p>
3. I Installed / Enabled IIS in Windows WITH CGI
World Wide Web Services -> Application Development Features -> [X] CGI.</p>
  This ensures the osTicket system can actually run on Windows. It allows the server to execute scripts such as PHP, the language osTicket is written in.
  </p>

</p>
<br />

<p>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/c4a10d6f-9898-490c-934d-4617b24e564f" />

</p>
<p>
4. Here we registered PHP from within IIS </p> This step connects IIS(the web server) to the PHP interpreter so it knows how to process PHP files.
</p>
</p>
<br />

<p>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/9c821bd8-ac97-4843-afc5-478fd171108b" />

</p>
<p>
5. Now, we installed HeidiSQL. </p> HeidiSQL provides a graphical interface to view and edit the database. This essentially makes the behind-the-scenes management much safer and easier allowing us to set up tables, users, and permissions much more easily.
</p>
<br />
<p>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/4f310d12-0c18-4a7d-9f4e-ee4efd367121" />



</p>
<p>
Inside Heidi SQL, I created a database called "osTicket." This serves as the central database to store all tickets, user data, and system configurations for the help desk system.
</p>
<br />
<p>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/3a6d3ff0-df9b-4da0-95a4-dd7813f28317" />
</p>
<p>
Finally, osTicket is fully installed. Now we can start managing support tickets and users.

</p>
<br />
