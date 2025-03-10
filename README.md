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

1. Enable Internet Information Services (IIS)
2. Install Web Platform Installer
3. Install MySQL and set up user and pass
4. Install C++ Redistributable
5. Configure permissions and install osTicket

<h2>Installation Steps</h2>
First you are going to create a Virtual machine, be sure to create a resource, name the resource group as well as the virtual machine name. Be sure to place your VM and resource group in the same region,(If place in different regions they will not be about to access one another). place images in windows 10, and the size to be atleast 2 VCPUS.
<P>
  
insert a Username and password within administrator account(this is for you solely to remember). click the Check box and Cream the VM
<p>
<img width="564" alt="image" src="https://github.com/user-attachments/assets/56902861-f981-47f9-8c32-a96397e06c62" />
<p>
<p>
<br />
<img width="619" alt="image" src="https://github.com/user-attachments/assets/d73378b9-831b-441c-8590-3fbb94b3e6fc" />
</p>
<p>
</p>
<img width="572" alt="image" src="https://github.com/user-attachments/assets/dabf8339-7739-4c85-94e9-7b43b41d8384" />
<p>
<p>    
</p>
<img width="647" alt="image" src="https://github.com/user-attachments/assets/88bda4f9-3d8e-4ab7-bb39-799d4b944fe6" />
<p>
<p>  
</p>
<img width="359" alt="image" src="https://github.com/user-attachments/assets/f890d9e5-5621-4e76-bff3-f54f6054f1b5" />


</p>
<p>
Once you create your virtual machine, it may take a moment to deploy. once the deployment is done, you can not start buy going to your desktop and open the virtual machine within your virtual desktop. 
</p>
<p>
<p>    
</p>
<img width="326" alt="image" src="https://github.com/user-attachments/assets/f74e21e7-c8af-447a-b995-40f46f9f1d92" />
<p>  
</p>
<p>
to gain access to the virtual desktop you now have to retreive the public IP address of the virtual machine and insert it into the remote desktop  
</p>
<p>  
</p>
<img width="100" alt="image" src="https://github.com/user-attachments/assets/bcebd823-de58-4a22-83f4-5975bbf982cb" />
<p>  
</p>
<img width="307" alt="image" src="https://github.com/user-attachments/assets/00228f6f-4256-4d5e-96ab-cb215bc2c11c" />
<p>  
</p>
</p>
this is where you enter the credentials, the username and password that you create within azures is what you want to insert here to gain access to the remote desktop
<p>
<p>
<img width="334" alt="image" src="https://github.com/user-attachments/assets/391bc2dc-7006-41fe-99d7-6b116a82a5b2" />
</p>
<p>
Within the Virtual machine, download the osTicket-Installation-Files.zip and unzip it onto your desktop, this will allow you to have the ability to install ostickets  
</p>
<p>
<img width="919" alt="image" src="https://github.com/user-attachments/assets/29ef9398-b57d-4e26-8e85-9c2358d94cd8" />

  
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
![image](https://github.com/user-attachments/assets/9664438d-6142-42ef-9fa0-57e26535d7af)
<P>
![image](https://github.com/user-attachments/assets/60241f8b-3a72-4f8b-89d7-5746989a5be1)
<p>
</p>
once it the file it downloaded, drag the file onto the desktop, right-click the file and press extract all.
</P>
<p>
![image](https://github.com/user-attachments/assets/69cbf8e7-d8e7-41f9-bf68-4703d57f4d53)
<p>
</p>
an unzipped version of the folder should now be present, now to enable IIS (internet information services) basically a web server that will be helping run ostickets.
<p>
you must first go to the control panel, within programs click on uninstall a program. nothing is going to be uninstalled this opens a window that we need to access windows features.
</p>
![image](https://github.com/user-attachments/assets/776a6737-664b-4398-a2a2-73e33a43ef73)
<p>
![image](https://github.com/user-attachments/assets/3786b0d8-9b80-424d-865e-b1bd0391b7f5)
<p>
![image](https://github.com/user-attachments/assets/b043e466-582a-439f-9591-d45a72f515e1)
<p>
once you click on the windows features, you will see internet information services, then world wide web services, then application development features and within that you will find CGI.
</p>
![image](https://github.com/user-attachments/assets/a347cf3d-f27d-432a-9d34-c40ee693313e)
<p>  
</p>
Next, from the osticket installation folder you download PHP manager for IIS (PHP is a backend web server language. OSticket runs off PHP so it is mandatory to be installed)
<p>
![image](https://github.com/user-attachments/assets/aa40d348-d145-4d83-a8b2-3836ea0b62d0)
<p>
within the same folder you are going to install the rewrite module.
</p>
![image](https://github.com/user-attachments/assets/976d6264-502a-4d58-a1b4-b6cda33d2dc7)
<p>
next you want to create a directory on the C drive titled PHP
</p>
![image](https://github.com/user-attachments/assets/dc0e6bee-ef21-4532-b24c-d10bb4e8f5c5)
</p>
![image](https://github.com/user-attachments/assets/82680bdd-e8f0-4c6a-a1d5-5e8469056945)
<P>
From the OSticketinstallation-folder you unzip the PHP PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) onto the C drive
<p>
to make things a bit easier, you right click to extract the folder. you go to the C drive and direct the extraction to the PHP folder  
</p>
![image](https://github.com/user-attachments/assets/bc53c2ba-ad5f-4cfd-95ee-d1ce1a712016)
</P>
From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.
</p>
![image](https://github.com/user-attachments/assets/421b88ac-3c2d-444c-9294-8d8013b5ae74)
</p>
From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi) lauch configuration windows after install and insert your own username and password.
</p>
![image](https://github.com/user-attachments/assets/9b19e60c-a980-4ecf-975a-c5fdf4c69120)
 </p>
 next you want to open IIS as an admin
</p>
<img width="362" alt="image" src="https://github.com/user-attachments/assets/a19d8a32-9de6-4ca6-92b5-67145957fdf9" />
<p>
register PHP from within IIS (the purpose of this to to make the web server know of the existance of PHP on the computer). to do so you have to click on the PHP manager we installed earlier. click register new PHP version. remember you placed it on the C drive in the PHP folder.
<p>
<img width="428" alt="image" src="https://github.com/user-attachments/assets/fbefa58c-1490-4c10-b2ee-0ae4e0c3a8e8" />
<p>
<img width="412" alt="image" src="https://github.com/user-attachments/assets/3bab238a-e824-42eb-bbc8-9cb6e58ee37d" />
<p>
now to reload IIS (stop and start)
<p> 

</p>

</p>
  
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
