<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com/watch?v=dEvGaxOgqf0)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure account
- Virutal Machine Running Windows
- osTicket Installation Files

<h2>Installation Steps</h2>
<h2>Step 1: Connect to your Virtual Machine with Remote Desktop</h2>
After creating a Virtual Machine in Azure, connect to it by entering the IP Adress into Remote Desktop and signing in.
<p>
<h2>Step 2: Enable IIS and CGI in Control Panel</h2>
  
 - Open the Control Panel app
 - Click on Programs > Turn Windows Features on or off
 - Find the Internet Information Services box and check it
 - Expand Internet Information Services>Expand World Wide Web Services>Expand Application Development>check the CGI Box
 - Hit OK and wait for everything to install
<img src="https://i.imgur.com/9xFOlkF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<h2>Step 3: Install all necessary osTicket Files</h2>

- First head to this [link](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6) to get the necessary files
- Start by downloading and insalling PHPManager and rewrite amd64
- Next Create a new folder on the root of the C drive called PHP
  <img src="https://i.imgur.com/ZragyLi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- Then extract the PHP Zip into the created PHP folder
  <img src="https://i.imgur.com/Sk5c8HB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- Next, download and install the VC_redist.x86.exe file and then MySQL
- After installing MySQL open the configuration wizard, Click Standard Configuration>Install as Windows Service>Create a password>Execute>Finish
- Next type IIS into the Windows search bar and open IIS as administrator
- Once Opened click on PHP Manager and then Register new PHP version
- Go to the created PHP folder and click php-cgi
   <img src="https://i.imgur.com/bPEQMgx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- Next go back to the IIS homepage and under Manage Server click on Restart
- Now download and extract the osTicket zip folder
- Grab the upload folder and put it in the wwwroot folder on the C drive
  <img src="https://i.imgur.com/pH5Zc8w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- Rename upload folder to osTicket
- Go back to IIS and restart the server again
- Next you will need to extract the osTicklet zip folder and drag the upload folder into wwwroot
  <img src="https://i.imgur.com/baxqiAv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- Now rename the upload folder to osTicket and reset the server in IIS
- After that find osTicket in the Connections tab of IIS and then go to Manage folder and click Browse *:80(http)
    <img src="https://i.imgur.com/tiST4o2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- If everything was installed correctly your screen should look like this
  <img src="https://i.imgur.com/15DqbLe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<h2>Step 4: Setting Up </h2>
<p>
</p>
<br />
