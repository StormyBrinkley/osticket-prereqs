<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Internet Information Services (IIS)
- PHP Manager
- Rewrite Module
- VC Redist
- MySQL
- Heidi SQL
- osTicket v1.15.8

<h2>Installation Steps</h2>
<p>
  Setting up osTicket on a Windows Virtual Machine:

**Create an Azure Virtual Machine Windows 10, 4 vCPUs**
Create the VM: Set-up a Windows 10 Virtual Machine on Azure, choose name, username, and password.
- Name: Vm-osticket
- Username: labuser (example)
- Password: osTicketPassword1! (example)
- If you are using MacOS then your need to install Microsoft Remote Desktop (MRD)
</p>

<p>
<img src="https://i.imgur.com/j9Y1wZd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
</p>
<p>
<h3>Step 1: Create and Prepare Your Virtual Machine</h3>
  
Install IIS: Open Windows Features and install Internet Information Services (IIS) with CGI and Common HTTP Features, and the IIS Management Console.

Set Up PHP: Create a directory C:\PHP, download PHP 7.3.8, and unzip it into C:\PHP.
</p>
<br />

<p>
<img src="https://i.imgur.com/Lo3tO6U.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/BKoa31J.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h3>Step 2: Install and Configure Components</h3>
  
Additional Tools: Download and install PHP Manager for IIS and the URL Rewrite Module.

Install MySQL: Download and install MySQL, using "Password1" as the root password.

Configure IIS for PHP: Open IIS, register PHP, and restart the IIS server.
</p>
<br />

<p>
<img src="https://i.imgur.com/welO5oY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<h3>Step 3: Set Up osTicket</h3>
  
Install osTicket: Download osTicket, move the "upload" folder to c:\inetpub\wwwroot, and rename it to "osTicket".

Enable PHP Extensions: In IIS, enable the extensions php_imap.dll, php_intl.dll, and php_opcache.dll.

Finalize Setup: Rename the ost-sampleconfig.php file, set permissions, and follow the browser setup to complete the osTicket installation. 

Create a database in HeidiSQL, then finish the setup with MySQL details. 

<p>
<img src="https://i.imgur.com/SarSvyz.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/F5Ds9Uo.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
Congrats! You have now successfully installed and setup osTicket!
</p>
<p>
<img src="https://i.imgur.com/sfVqSY0.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>

</p>
<br />


