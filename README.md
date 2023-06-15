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

- Enable GCI,IIS.
- Download PHP ManagerForIIS_V1.5.0.msi.
- Download rewrite_amd64_en-US.msi (Rewrite Module).
- Download PHP 7.3.8
- Download VC_redist.x86.exe (MS visual C++ ).
- Download my SQL server.
- Open IIS as an Admin,Register PHP from within IIS.
- Dowload osTicket (osTicket-v1.15.8.).
- Enable Extensions.
- Rename: ost-config.php.
- Assign Permissions: ost-config.php.
- Continue Setting up osTicket in the browser.
- Download Heidi SQL (HeidiSQL_12.3.0.6589_Setup.exe).
- Congratulations,it is installed.
- Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php

 

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/gXex0rY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once you connect your virtual machine to Remote desktop connection, simply go to control pannel and click turn windows features on or off, then enable internet information services, Application development features and check GCI box and common HTTP features.
</p>
<br />

<p>
<img src="https://i.imgur.com/u4yTnx2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download PHP ManagerFORIIS_V1.5.0.msi and run the file.
</p>
<br />

<p>
<img src="https://i.imgur.com/hUqutbB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download rewrite_amd64_en-US.msi (Rewrite Module) and install it.
</p>
<br />

<p>
<img src="https://i.imgur.com/Yn7Y1mj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download php-7.3.8-nts-Win32-VC15-x86.zip and go to the top right hand side click 3 dots and click keep it and then keep anyway.
</p>
<br />

<p>
<img src="https://i.imgur.com/XJbRtup.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Make a new PHP folder on C/:Drive, Go to the -> downloads folder right click the -> PHP 7.3.8 folder which you just downloaded and unzip/extract into the C/:Drive folder of PHP.
</p>
<br />

<p>
<img src="https://i.imgur.com/qLeQnTu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download VC_redist.x86.exe (MS visual C++ ) open file and install it.
</p>  
<br />

<p>
<img src="https://i.imgur.com/7BEdL50.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download mysql-5.5.62-win32.msi (My SQL server).
</p>  
<br />

<p>
<img src="https://i.imgur.com/2u8I9zq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After click "Next" make sure you select Typical.
</p>
<br />

<p>
<img src="https://i.imgur.com/WZnPJfu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Launch Configuration Wizard (after install) click finish, new tab will going to open than select Standard Configuration.
</p>
<br />

<p>
<img src="https://i.imgur.com/uULfo7p.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Write it down a new root password Example: "Password1" make sure you don't forget your password, keep it remember.
</p>
<br />

<p>
<img src="https://i.imgur.com/OKaqfwK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to the "Type to search" bar next to the windows icon, type IIS click right and run as a Admin, double click on "PHP Manager" and resgister new PHP version from within IIS.After click on Register new PHP version, Click on 3 dots and go to the C/:Drive PHP folder that we make previously than click php-cgi.
</p>
<br />

<p>
<img src="https://i.imgur.com/f852oAe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After the PHP Register, Go to the left side on the top and click on "osticket" and restart the Manage server on the right side.
</p>
<br />

<p>
<img src="https://i.imgur.com/kDzpfm9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download osTicket (osTicket-v1.15.8.) go to the downloads folder and open osTicket downloaded folder,it's going to be 2 folders inside the osTicket folder 1- "upload", 2- "Scripts". Go to the File explore -> C/:Drive click on -> inetpub folder then -> wwwroot folder and move the "upload" folder into the wwwroot by simply drag and drop and rename Upload folder to "osTicket". 
</p>
<br />

<p>
<img src="https://i.imgur.com/bVpR96s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server) Go to sites -> Default -> osTicket On the right, click “Browse *:80” and the new tab will open you can see osTicket Installer,in order to continue enable a few extensions mark as " X " Cross
</p>
<br />

<p>
<img src="https://i.imgur.com/f2qn9Ij.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to IIS, sites -> Default -> osTicket  Double-click PHP Manager Click “Enable or disable an extension” Note that some extension are not enable.
</p>
<br />

<p>
<img src="https://i.imgur.com/A4NGCI2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable: php_imap.dll -> Enable: php_intl.dll -> Enable: php_opcache.dll.
</p>
<br />

<p>
<img src="https://i.imgur.com/sR4sTSn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Refresh the osTicket site in your browse, observe the changes and click continue.
</p>
<br />

<p>
<img src="https://i.imgur.com/2bQ9Isa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to C:\Drive ->inetpub ->wwwroot ->osTicket ->include ->ost-sampleconfig.php, Rename: ost-config.php
</p>
<br />

<p>
<img src="https://i.imgur.com/EGESdUy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Assign Permissions: ost-config.php ->Security ->Advance ->Disable inheritance -> Remove All.
</p>
<br />

<p>
<img src="https://i.imgur.com/SSqsoYp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
New Permissions ->Add ->"click Select a principal on the top" -> write it down Everyone and click on Check Names ->Check all the unchecked boxes and click OK.
</p>
<br />

<p>
<img src="https://i.imgur.com/QVwmDTz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click Continue and keep Setting up osTicket in the browser ->Name Helpdesk ->Default email(receives email from customers) ->Username ->Password.
</p>
<br />

<p>
<img src="https://i.imgur.com/9seakMs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download Heidi SQL ->Next ->Install ->Finish.
</p>
<br />

<p>
<img src="https://i.imgur.com/SYFUVm1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a new session ->root ->Use the same passowrd of MYSQL Example: "Password1" and click Open.
</p>
<br />

<p>
<img src="https://i.imgur.com/Mul0ODu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Connect to the session, right click Unnamed ->Create new,Create a database called “osticket”
</p>
<br />

<p>
<img src="https://i.imgur.com/SIM0Tp7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a new database Name: "osticket"
</p>
<br />

<p>
<img src="https://i.imgur.com/PS2m6SA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Write it down the Database just created "osticket" into "osTicket System Installer" make sure you use the same user and password of MYSQL and click Install Now.
</p>
<br />

<p>
<img src="https://i.imgur.com/QDDIeK9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Congratulations, it is installed.Browse to your help desk login page:http://localhost/osTicket/scp/login.php End Users osTicket URL: http://localhost/osTicket/ Login with your Username and password which you set up.
</p>
<br />

<p>
<img src="https://i.imgur.com/LfBl8k1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Welcome to osTicket - (Admin Panel)
</p>
<br />


<p>
<img src="https://i.imgur.com/kiEqpOj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Clean up,Go to C:\Drive ->inetpub ->wwwroot ->osTicket -> Delete "Setup folder",Set Permissions to “Read” only: C:\Drive inetpub ->wwwroot ->osTicket ->include ->ost-config.php ->right click & properties->Security & Advanced -> click Everyone then Edit set a permisson by uncheck all boxes and leave Checked Read & execute , Read -> Apply and Ok. Enjoy using osTicket System!!

</p>
<br />


