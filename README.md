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

- Azure Virtual machine
- Internet Information Services(IIS)
- PHP Manager
- Rewrite Module
- VC Redist
- MySQL
- Heidi SQL
- osTicket v1.15.8
- This is the link to download everything: https://drive.usercontent.google.com/download?id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD&export=download&authuser=0
<h2>Installation Steps</h2>

<h2>Step 1: Create a Virtual Machine</h2>

<p>
<img src="https://github.com/user-attachments/assets/0baad5d2-daf8-4e4d-9492-6eb666e08e13" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to Microsoft Azure.
Set up a virtual machine with the following specifications:
Operating System: Windows 10 Pro, version 22H2.
Minimum Requirements: At least 2 vCPUs and 16 GB of memory.
Ensure your virtual machine meets these specifications for optimal performance.
</p>
<br />
<h2>Step 2: Connect to the Virtual Machine</h2>

<p>
<img src="https://github.com/user-attachments/assets/33f98071-548f-4155-a311-b4679e136896" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Use the public IP address assigned to your virtual machine.
Open the Remote Desktop Connection application on your computer.
Enter the public IP address and establish a connection to access the virtual machine.
</p>
<br />

<h2>Step 3: Download Required Files</h2>

<p>
<img src="https://github.com/user-attachments/assets/0a321d21-aca9-4a8e-87f2-0b411903530f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once logged into the virtual machine, open Microsoft Edge.
Paste the following link into the browser:
https://drive.usercontent.google.com/download?id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD&export=download&authuser=0
Download the necessary files from the folder and open them
Make sure to save the files in an easily accessible location on your virtual machine.
</p>
<br />

<h2>Step 4: Extract and Organize Installation Files</h2>

<p>
<img src="https://github.com/user-attachments/assets/60b5f1a1-9375-4561-b9da-c9489c669dc1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After downloading the files, click on the folder icon at the bottom of the screen to open the Downloads folder.
Locate the downloaded files, then drag them onto the desktop for easy access.
Right-click the downloaded file and select Extract All.
Ensure the extraction path is set to:
C:\Users\labuser\Desktop\osTicket-Installation-Files
Click Extract to complete the process.
This will ensure that the installation files are properly organized and ready for use.
</p>
<br />

<h2>Step 5: Install the Web Server (IIS)</h2>

<p>
<img src="https://github.com/user-attachments/assets/0f170bb6-e027-4cc9-97a2-ed81d2aeac8c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to the bottom of the screen, click on Search, and type in Control Panel.
Once in the Control Panel, click on Uninstall a program.
On the left-hand side, click on Turn Windows features on or off.
In the window that opens, expand Internet Information Services -> Application Development Features.
Check the box for CGI to enable it.
Click OK to apply the changes.
This will install the necessary web server components for the osTicket installation.
</p>
<br />

<h2>Step 6: Verify IIS Installation</h2>

<p>
<img src="https://github.com/user-attachments/assets/bf2688d4-8381-42d6-95d0-6bc126424f66" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To confirm that IIS (Internet Information Services) is correctly installed:

Open Microsoft Edge on your VM.
In the address bar, type 127.0.0.1 and press Enter.
If IIS is installed correctly, you should see the IIS welcome page. This indicates that the web server is functioning properly.
</p>
<br />

<h2>Step 7: Install PHP Manager</h2>

<p>
<img src="https://github.com/user-attachments/assets/bcdfec74-a0fe-4384-b0f3-4e0905c53650" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to the osTicket-Installation-Files folder on your Desktop.
Double-click the PHP Manager setup file to begin the installation process.
Click Next to proceed.
Read and agree to the terms by selecting I Agree, then click Next.
Continue clicking Next until the installation is complete.
</p>
<br />

<h2>Step 8: Install URL Rewrite</h2>

<p>
<img src="https://github.com/user-attachments/assets/c86bd02a-33ba-46dc-b885-ca4a95ea6244" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the osTicket-Installation-Files folder on your Desktop, locate and click on URL Rewrite.
Proceed by agreeing to the terms and conditions, selecting I Agree.
Follow the prompts and click Next to complete the installation.
</p>
<br />

<h2>Step 9: Create the PHP Directory</h2>

<p>
<img src="https://github.com/user-attachments/assets/cc458cd1-7fa8-403d-92e1-9a3a41c69cad" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to the bottom of the screen and right-click the Folder icon, then select File Explorer.
In File Explorer, navigate to Windows (C:).
Right-click inside the folder and select New > Folder.
Name the new folder PHP.
</p>
<br />

<h2>Step 10: Unzip PHP 7.3.8 into the PHP Folder</h2>

<p>
<img src="https://github.com/user-attachments/assets/8c8eace9-2177-48a4-a0cd-7f40e7018f48" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to the osTicket Installation Files folder on your desktop.
Right-click the php7.3.8 folder and select Extract.
In the Browse for Folder window, navigate to Windows (C:), then select the PHP folder that was created earlier.
Click Extract to unzip the contents of php7.3.8 into the C:\PHP folder.
</p>
<br />

<h2>Step 11: Install Visual C++ Redistributable (vc_redist)</h2>

<p>
<img src="https://github.com/user-attachments/assets/726a50c5-3607-4544-b1dc-3c24fe030cc9" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to the osTicket Installation Files folder on your desktop.
Locate and double-click on the vc_redist file to begin the installation process.
Follow the on-screen instructions to complete the installation. Make sure to accept the terms and allow the installation to finish.
</p>
<br />

<h2>Step 12: Install MySQL</h2>

<p>
<img src="https://github.com/user-attachments/assets/8db5d656-dad7-4b31-8f3f-77a6cb0f6154" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the osTicket Installation Files folder on your desktop, locate and double-click on the mysql installer to begin the setup process.
Follow the prompts and agree to all terms and conditions until you reach the Setup Types screen.
Select the Typical setup type, then continue agreeing to everything until you reach the final setup screen.
When the installation is complete, make sure to check the option to Launch MySQL and click Finish to start MySQL.
</p>
<br />

<h2>Step 13: MySQL Configuration</h2>

<p>
<img src="https://github.com/user-attachments/assets/3728bfd5-3ed3-44a3-8363-a3ea63d972d5" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once MySQL launches, you will be prompted to configure the server. Select Standard Configuration and click Next.
URGENT: For the Username and Password, type root for both fields. Be very careful with this step, as incorrect credentials here can cause issues later. After entering the information, click Next.
On the following screen, click Execute to apply the configuration.
</p>
<br />

<h2>Step 14: IIS Configuration for PHP</h2>

<p>
<img src="https://github.com/user-attachments/assets/9916ec29-1970-479d-b5b3-f3efd604433d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to the Search bar at the bottom-left of the screen, type IIS, right-click it, and select Run as Administrator.
In the IIS Manager window, click on PHP Manager.
Under PHP Manager, click Register PHP version.
A file explorer window will appear. Click the three dots (…) and navigate to C:\PHP.
Select php-cgi.exe, then click Open and OK.
</p>
<br />

<h2>Step 15: Restart IIS for Changes</h2>

<p>
<img src="https://github.com/user-attachments/assets/6472bddd-4321-4655-8e1c-481e1b1c860c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the IIS Manager window, locate your site (it may be named osticket-vm or similar).
Right-click on osticket-vm and select Stop.
Wait a moment, then right-click on osticket-vm again and select Start to restart the service.
</p>
<br />

<h2>Step 16: Extract and Place osTicket Files</h2>

<p>
<img src="https://github.com/user-attachments/assets/773ffb12-f5a1-4345-840d-590f10611386" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right-click the osTicket folder and select Extract.
Open a second File Explorer window (if one is not already open).
Navigate to C:\inetpub\wwwroot.
Drag and drop the upload folder from the osTicket Installation Files folder into wwwroot.
Rename the folder to osTicket. Make sure the capitalization is correct—osTicket (with a capital "T" and no spaces between "os" and "Ticket"). This is case-sensitive and will be important for the future steps.
</p>
<br />

<h2>Step 17: Restart the osTicket VM in IIS</h2>

<p>
<img src="https://github.com/user-attachments/assets/a4f7d970-2e03-41e6-8e45-dc431f66c5cc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS Manager.
In the Connections panel, right-click on osticket-vm.
Click Stop and wait a few moments.
After a short wait, right-click again on osticket-vm and click Start to restart the virtual machine.
</p>
<br />

<h2>Step 18: Verify osTicket Website Load

</h2>Step 18: Verify osTicket Website Load</h2>

<p>
<img src="https://github.com/user-attachments/assets/102bacb1-8828-4485-91bf-e9d187c72ab2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In IIS Manager, expand osticket-vm.
Expand Sites and click on osTicket.
On the right-hand side, click *Browse :80.
The osTicket website should now load in your default browser.
</p>
<br />

<h2>Step 19: Enable Required PHP Extensions</h2>

<p>
<img src="https://github.com/user-attachments/assets/4e577d96-bfbd-4a02-a792-233f12c0deb1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to IIS Manager and expand osticket-vm.
Expand Sites and click on Default Web Site.
Then, click on osTicket and select PHP Manager.
Click on Enable or Disable Extensions.
Enable the following extensions:
php_imap
php_intl
php_opcache
After enabling these extensions, go back to the osTicket webpage and refresh it.
You should now see checkmarks next to the previously unchecked items.
</p>
<br />

<h2>Step 20: Rename Configuration File</h2>

<p>
<img src="https://github.com/user-attachments/assets/8d809f20-6ff2-45ba-a829-3b88e3b25c38" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open File Explorer and navigate to C:\inetpub\wwwroot\osTicket.
Go to the include folder and locate the file ost-sampleconfig.php.
Right-click on ost-sampleconfig.php and select Rename.
Rename the file to ost-config.php (make sure the capitalization and spelling are exact).
Press Enter to confirm the name change.
Note: The file name is case-sensitive, so ensure that it matches exactly as described.
</p>
<br />

<h2>Step 21: Modify File Permissions</h2>

<p>
<img src="https://github.com/user-attachments/assets/60e31343-d606-4151-af96-a2486ac5aa63" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right-click on ost-config.php and select Properties.
In the Properties window, go to the Security tab.
Click on Advanced.
In the Advanced Security Settings window, click on Disable inheritance.
In the pop-up, select Remove all inherited permissions from this object and click OK.
Click on Add to create new permissions.
In the Permission Entry window, click Select a principal.
Type Everyone and click Check Names, then click OK.
In the Basic Permissions section, check Full Control.
Click OK, then click Apply, and OK again to confirm the changes.
These steps ensure the correct permissions are set for the configuration file.
</p>
<br />
<h2>Step 22: Install Database and Configure osTicket</h2>
<p>
<img src="https://github.com/user-attachments/assets/4e51cce9-5815-4782-a863-bb2c5ee9033e" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to the osTicket webpage and click Continue.

Fill out all the fields to your preference.

When you reach the Database Settings section:

Open the osTicket Installation folder.
Locate and click on HeidiSQL.
Agree to all terms and conditions, then click Install.
Ensure that Launch HeidiSQL is checked and click Finish.
Once HeidiSQL opens:

Click Skip if prompted.
Click New (a green circle) at the top.
In the Password field, enter the password you set for MySQL during installation.
Click Open to connect to the database.
In the HeidiSQL window:

Right-click on Unnamed in the left-hand panel and select Create New.
Choose Database.
Name the database as osTicket (case-sensitive: no space and capital "T").
Click OK to create the database.
Return to the osTicket webpage and in the MySQL Database section:

Enter osTicket as the database name.
Input your username and password.
Click Install Now to complete the installation process.
This step finalizes the database setup and completes the installation.
</p>
<br />
<H2>FINALLY DONE</H2>
<p>
<img src="https://github.com/user-attachments/assets/2cdc4fd6-6509-422c-94bf-e07f0c07f9fd" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
CONGRADULATIONS YOU INSTALLED OSTICKET
</p>
<br />
