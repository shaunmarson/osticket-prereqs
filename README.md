<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
Hello, everyone! My name is Shaun A. Marson, and I’m an IT Professional with experience in a variety of systems and technologies. Today, I’ll be showing you how to set up osTicket, a widely used open-source support ticket system. This guide will help you get your osTicket installation up and running quickly. Let’s get started!.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Prerequisites</h2>

Prerequisites:

Ensure you have a web server (Apache or Nginx).
PHP version 5.6 or later installed.
A MySQL database server running.
"Before we begin, make sure you have the following:

A web server set up on your machine or hosting service (Apache or Nginx recommended).
PHP 5.6+ installed.
A MySQL database server running."
Download osTicket:

Visit the official osTicket website: https://osticket.com/download/
Download the latest stable version.
"First, you’ll need to download the latest version of osTicket from the official site."

Extract and Upload Files:

Extract the downloaded ZIP file.
Upload the files to your server, preferably to a folder like /var/www/osticket or any directory where you host your web applications.
"Once downloaded, extract the files and upload them to your server. For example, if you're using a Linux server, you can place them in /var/www/osticket."

Create a MySQL Database:

Access your MySQL server and create a database for osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a MySQL Database
You need to create a MySQL database for osTicket. Here’s how you can do it:

a. Access MySQL:
Log in to MySQL (or MariaDB) as the root user

b. Create the database and user:
Run the following commands in the MySQL shell to create the database and a new user
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start osTicket Installation via Web Browser
Open your browser and navigate to the osTicket directory where you uploaded the files. For example, if you uploaded the files to http://yourdomain.com/osticket, type that URL in your browser.

You should see the osTicket installation page. Follow these steps:

a. Welcome Page:
Click on "Next" to start the installation.

b. License Agreement:
Agree to the terms by clicking "I Agree".

c. System Configuration:
Enter your MySQL database details:

Database Host: localhost (or the IP address of your database server).
Database Name: osticket
Database Username: osticket_user
Database Password: your_password (the password you set up).
Set the Admin Email, which will be used for notifications.

d. Directory Permissions:
The installer will check your system’s permissions. Ensure the following directories are writable (if not, update the permissions):

include/
attachment/
scp/
plugins/
For example, on Linux systems, you can run

e. Configuration Settings:
Admin Username: Set a secure admin username.
Admin Password: Set a secure password for the admin account.
Admin Email: Provide the admin’s email address.
Click "Install Now" to proceed.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finalizing Installation
Once the installation is complete, you’ll see a success message. At this point, the installation files are still present, and the installer will prompt you to delete the setup folder for security reasons.
You can either manually delete it or click "Delete Now" from the installation page.

Access Admin Panel
After successful installation, you can log in to the osTicket Admin Panel using the admin credentials you just created.
Go to: http://yourdomain.com/osticket/scp (Replace yourdomain.com with your domain or IP address).

Configure osTicket
Now that osTicket is installed, you can start configuring:

Set up departments, agents, and teams.
Customize your email templates and ticket forms.
Configure auto-response emails and helpdesk rules.


Conclusion:
Congrats! You’ve now installed and set up osTicket. You can start using it to manage support tickets. Let me know if you need help configuring or troubleshooting!
</p>
<br />
