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
- Dowload osTicket (osTicket-v1.15.8.)

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
Download osTicket (osTicket-v1.15.8.) go to the downloads folder and open osTicket downloaded foler,it's going to be 2 folders inside the osTicket folder 1- "upload", 2- "Scripts". Go to the File explore -> C/:Drive click on -> inetpub folder then -> wwwroot folder and move the "upload" folder into the wwwroot by simply drag and drop and rename Upload folder to "osTicket". 
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
<img src="https://i.imgur.com/uULfo7p.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Write it down a new root password Example: "Password1" make sure you don't forget your password, keep it remember.
</p>
<br />
