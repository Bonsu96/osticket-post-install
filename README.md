 
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket  Post Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

<h2>Configuration Steps</h2>

1. Access Azure Portal:

2. Log in to the Azure Portal (https://portal.azure.com/).
Create a Virtual Machine (VM):

3. Create a new Virtual Machine where you plan to host osTicket. Configure the VM settings, including size, storage, and networking.
Install a Web Server:

4. osTicket requires a web server. You can choose Apache or Nginx. Install and configure the web server on your VM.
Install PHP:

5. Install PHP on your VM. osTicket requires PHP to function. Ensure you install the required PHP extensions as well.
Install a Database Server:

6. Choose a database server (e.g., MySQL or MariaDB) and install it on your VM. Create a database and a user for osTicket.
Download and Extract osTicket:

7. Download the latest version of osTicket from the official website (https://osticket.com/download/). Upload it to your VM and extract the files.
Configure osTicket:

8. Navigate to the osTicket directory and find the include/ost-config.php file. Follow the instructions in the file to configure your database settings, mail settings, and other options.
Set Permissions:

9. Adjust the file and directory permissions to ensure that the web server can read and write to necessary files and directories. Refer to osTicket documentation for specific permission requirements.
Access osTicket Installation Wizard:

10. Open your web browser and navigate to the osTicket installation wizard (e.g., http://your_vm_ip/osticket). Follow the on-screen instructions to complete the installation.
Create an Admin Account:

11. During the installation, you'll be prompted to create an administrator account for osTicket. Provide the required information to set up the admin account.
Remove Installation Directory:

12. After the installation is complete, remove the setup directory from your osTicket installation. This is a security measure to prevent unauthorized access to the setup scripts.
Configure Email Settings:

13. Configure email settings within osTicket to ensure that email notifications and replies work correctly. This typically involves specifying your SMTP server details.
Set Up CRON Jobs:

14. Configure any necessary CRON jobs for osTicket. These jobs are essential for automating certain tasks, such as fetching emails and sending notifications.
SSL Configuration (Optional):

If you are using osTicket in a production environment, consider setting up SSL for secure communication. You can obtain an SSL certificate and configure your web server accordingly.
Test osTicket:

Perform thorough testing to ensure that osTicket is functioning as expected. Create and respond to tickets, test email notifications, and verify that all features are working correctly.
Backup and Monitoring:

Regularly back up your osTicket installation and set up monitoring to keep track of system performance and detect potential issues.




