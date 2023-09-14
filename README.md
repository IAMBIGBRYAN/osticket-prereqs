<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

Setting up osTicket on Microsoft Azure involves creating a virtual machine (VM), configuring the necessary software components, and then installing osTicket. Here's a step-by-step guide:

1. Create an Azure Virtual Machine

Log in to your Microsoft Azure portal: https://portal.azure.com/.

Click on "Create a resource."

Search for "Ubuntu Server" in the Azure Marketplace, and select it.

Configure the VM settings, including the size, authentication, and other details as needed.

Create the VM. Azure will provision the virtual machine for you.

![image](https://github.com/IAMBIGBRYAN/osticket-prereqs/assets/144714236/3ae803a8-3d4e-4ea6-b488-8f2551edba0a)


2. Connect to the Azure VM

Once the VM is created, you can connect to it using SSH. You can use tools like PuTTY (for Windows) or the terminal (for macOS and Linux).

3. Update the System

After connecting to the VM, update the package list and upgrade the installed packages

4. Install Apache, MySQL, PHP

Install Apache, MySQL (or MariaDB), and PHP on your Azure VM

5. Create a Database for osTicket

Log in to MySQL as the root use
Create a new database and user for osTicket

![image](https://github.com/IAMBIGBRYAN/osticket-prereqs/assets/144714236/bff0b897-0c8e-465b-b3f2-ebd6b00fa6c2)


6. Download and Install osTicket:

Download the latest version of osTicket to your Azure VM:
Unzip the osTicket archive and move it to the web server directory

7. Configure osTicket
   Rename the ost-config.sample.php file to ost-config.php
   Edit the ost-config.php file to configure your database settings

8. Set Permissions
   Set the correct permissions on the osTicket files and directories

 9. Complete the Installation:

Open a web browser and navigate to your osTicket installation by entering your Azure VM's public IP address or domain name:

Follow the on-screen instructions to complete the installation. Create an admin account and configure your help desk settings.

Once the installation is complete, delete the setup directory

10. Secure Your osTicket Installation
    ![image](https://github.com/IAMBIGBRYAN/osticket-prereqs/assets/144714236/4212f4b4-8c07-4c9b-ac9c-7473afce63c3)

 

Ensure that your server's firewall in Azure is configured to allow only necessary ports (e.g., 80 and 443).

Consider setting up SSL/TLS for secure HTTPS access to your osTicket installation.

That's it! You've now successfully set up osTicket on a Microsoft Azure Virtual Machine. Remember to regularly back up your data and keep both the server and osTicket software updated for security and stability.
