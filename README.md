<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>
<p>
  Setting up osTicket on a Windows Virtual Machine:

**Create an Azure Virtual Machine Windows 10, 4 vCPUs**
- Name: Vm-osticket
- Username: labuser (example)
- Password: osTicketPassword1! (example)

</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 1: Create and Prepare Your Virtual Machine</h2>
  
Create the VM: Set up a Windows 10 Virtual Machine on Azure, choose name, username like "labuser" and a password like "osTicketPassword1!".
  
Install IIS: Open Windows Features and install Internet Information Services (IIS) with CGI and Common HTTP Features, and the IIS Management Console.

Set Up PHP: Create a directory C:\PHP, download PHP 7.3.8, and unzip it into C:\PHP.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 2: Install and Configure Components</h2>
  
Additional Tools: Download and install PHP Manager for IIS and the URL Rewrite Module.

Install MySQL: Download and install MySQL, using "Password1" as the root password.

Configure IIS for PHP: Open IIS, register PHP, and restart the IIS server.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 3: Set Up osTicket</h2>
  
Install osTicket: Download osTicket, move the "upload" folder to c:\inetpub\wwwroot, and rename it to "osTicket".

Enable PHP Extensions: In IIS, enable the extensions php_imap.dll, php_intl.dll, and php_opcache.dll.

Finalize Setup: Rename the ost-sampleconfig.php file, set permissions, and follow the browser setup to complete the osTicket installation. 

Create a database in HeidiSQL, then finish the setup with MySQL details. 

</p>
<br />


